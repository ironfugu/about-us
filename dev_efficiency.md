## Measuring Productivity

There was a great talk by the CTO of CircleCI talking about creating high performance teams and he gave these 3 key take aways.

* Invest in your effectiveness - take the time to be more efficient
* Own your story - tell the story you want about your productivity, and don't let others do it for you
* Share - share the data openly

## Packet Formula for Effectiveness

At Packet, we want to measure effectiveness but also drive home core behaviors we care about.  Two that are easier to measure is caring and taking small steps.  Here are the two factors to measure

* Time to live for PRs (time from PR Open to Push to Prod)
* Number of Rollbar errors per day for that service

The first repo we will use is [api](https://github.com/packethost/api) since this affects the most squads currently.  One decision to make is, what is an acceptable TTL?  The API service is probably the worst because it takes over 2 hours to test.  Also, it takes a bit of time to deploy due to its workers, so currently doing CD is nearly impossible.

__TTL Considerations__

* Time to Review - people can get busy, but the idea is that your squad members should be available to review your code within 4 hours, and code reviews could take up to an hour
* Time to Build/Test - this is how long it practically takes to build/test the repo, for API, its about 2 hours (this can be done in parallel to the build)
* Time to Push to Prod - API "server" deploys can be done fairly quickly, and takes about 10-15 minutes.  However, the workers currently has to be manually scheduled, and done, so including time for people to find time and then wait, we can peg this at 2 hours.

So, currently, the practical TTL for API would be around 6-7 hours (assuming review and test time are done concurrently).  So, is 6-7 hours acceptable?  This probably should be considered ok but not ideal.  We really want to get to 2-3 hours and eventually down to 1 hour.  So let say, if 1 hour is considered 100%, each hour after should deduct 10%.  Second, rollbar errors, we don't want to push code thats faulty, and we should just let errors linger without any care.  So, assuming 0 rollbar errors is 100%, let's just deduct 1% per rollbar error (RE).

```
((100 - MIN((10 * (AVG(TTL)-1))),200) + (100 - MIN(RE, 200)) = PFE
```

So, lets say we have 5 PRs, and they average out to 6.5 hours, and we have 45 rollbar errors.  Then the formula is
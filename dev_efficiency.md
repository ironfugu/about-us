## Measuring Productivity

There was a great talk by the CTO of CircleCI talking about creating high performance teams and he gave these 3 key take aways.

* Invest in your effectiveness - take the time to be more efficient
* Own your story - tell the story you want about your productivity, and don't let others do it for you
* Share - share the data openly

## (WIP) Packet's View of Effectiveness

At Packet, we want to measure effectiveness but also drive home core behaviors we care about.  Two that are easier to measure is caring and taking small steps.  Here are the two factors to measure

* Time to live for PRs (time from PR Open to Push to Prod)
* Number of Rollbar errors per day for that service

The first repo we will use is [api](https://github.com/packethost/api) since this affects the most squads currently.  One decision to make is, what is an acceptable TTL?  The API service is probably the worst because it takes over 2 hours to test.  Also, it takes a bit of time to deploy due to its workers, so currently doing CD is nearly impossible.

__TTL Considerations__

* Time to Review - people can get busy, but the idea is that your squad members should be available to review your code within 4 hours, and code reviews could take up to an hour
* Time to Build/Test - this is how long it practically takes to build/test the repo, for API, its about 2 hours (this can be done in parallel to the build)
* Time to Push to Prod - API "server" deploys can be done fairly quickly, and takes about 10-15 minutes.  However, the workers currently has to be manually scheduled, and done, so including time for people to find time and then wait, we can peg this at 2 hours.
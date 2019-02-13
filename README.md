Welcome to our development culture document.  Here describes how we view the world and behaviors and ideals that make you successful here at Packet

### Our Mission

`Any hardware combination, any OS, any location, in our DC or yours, 100% successful provisions under 60 seconds`

### Our Company Core Values

* We are excited about leading our industry.
* We are driven, ambitious and persistent people.
* We find creative solutions to hard problems.
* We are effective at getting things done the right way.
* We are community minded and do the right thing.

### Our Team Culture

Teammates driven by [Autonomy, Mastery and Purpose](https://en.wikipedia.org/wiki/Drive:_The_Surprising_Truth_About_What_Motivates_Us) working together with [psychological safety](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html) is the basis for everything we do.

### Done right through Core Behaviors

 * __Care about...__ - This is the most important behavior as all other behaviors depend on this
      * Care about the craftmanship of your work.
      * Care about Packet.
      * Care about your coworkers and their success.
      * Care about standards or quality.
      * Care about learning and growing your skills.

 * __Take small purposeful steps__ - We are doing some great things, but we can only get there one commit at a time.
      * Understand "what" the problem statement is and how it impacts the user or customer
      * Think "[how](https://blog.crisp.se/wp-content/uploads/2016/01/mvp.png)" can I do this in incremental steps, by providing useful functionality along the way.
      * Expect __failure__ along the way and feel the freedom to experiment to find the right solution
      * Practice makes perfect

 * __Listen then collaborate__ - Listen to understand, rather than to respond
      * Listen with empathy, understand the other's point of view
      * Give your full attention
      * Give space for others to respond
      * Understand how your work will/can impact others
     
 * __Provide Continuous Feedback & Progress__ - effective communications is really hard, but essential to our work
      * Providing useful and timely comments and suggestions in code and processes
      * Keep others informed of your progress through our issue tracking tool
      * Be open and honest, don't say something you don't actually believe or feel
      * When providing feedback to others
        * Be Specific and timely
        * Give compliments openly, critiques privately
        * Use the ["when you, I feel..."](https://www.erikbohlin.net/handouts/Constructive_Feedback.pdf) form of feedback

 * __Seek learning and be uncomfortable__ - Don't get complacent, find new ways to do things
      * Don't pick a path just because its easy or comfortable
      * Pick the right tool for the job
      * There's always multiple ways to do something, explore them    
      * Seek guidance from others, don't have the "invented here" mentality

If you retain anything from this article, it is the core behaviors from above.  We live by this, we [hire](interview.md) based on this and evaluate [performance](perf.md) based on this.  If you excel at those, you will go far in Packet SWE.

### How and why we do it

Here are things we specifically do to help achieve our mission

__Code__

What   | Reasoning | Tooling
:------- | ----- | ---------
(Near) Atomic Changes | Pushing smaller changes allows us to deliver incremental value; also reduces chance of breakage | GitHub
High code coverage | CI is useless without good quality coverage, and we can't ship to production confidently without it | Drone
Refactor constantly | Reduce code debt on every issue you work on | GitHub, Rubocop

__Docs__

What   | Reasoning | Tooling
:------- | ----- | ---------
Branches and PRs | introduce small changes safely, ensure the code fits our philosophy, knowledge sharing | GitHub, Jira, Slack
Effective documentation | moving quickly means we work on a lot of different things, document for future teammates or yourself | GitHub Markdown, Jira, Confluence
Aligned Development | Make sure what we're working on brings business value | Trello, Jira

__DevOps__

What   | Reasoning | Tooling
:------- | ----- | ---------
Tight CI/CD | The way we can ship the code quickly and confidently | GithHub, Drone, Quay.io, Hashistack
Automated System/UI Testing | Once code is in production, is it really working?  Running things like Runscope against the API gives us confidence that new changes didn't mess up prod | Runscope
DevOps Culture| Everyone should know how stuff runs and keep an eye that services are working as expected | Rollbar, NewRelic, Hashistack

### Our Team

We've adapted the "Spotify" [model](https://blog.crisp.se/wp-content/uploads/2012/11/SpotifyScaling.pdf) for scaling our teams.  We have a few squads and are still experimenting with the right mix of people and skillsets.

A Squad is the smallest group of people, which is usually no bigger than 8 members. They are responsible for one key area. The Squad members have end-to-end responsibility. The freedom of their choices and decisions is limited by the company’s mission and by the product strategy. The Product Owner decides on the hierarchy of priorities for Squad members. They are responsible for small and frequent releases.
Each Squad has professionals which specialize in certain areas. All these people, who have the same responsibilities in separate Squads, are gathered in a group called a Chapter. An Engineering Manager is a line manager here. Everyone is a member of both a Squad and Chapter.

__Our Chapters__ 

Responsibilities| Engineering Manager
:-------------| ------------- 
Backend/API/Microservices (Software) |Josue
UX/UI (Software) | Linda
Infra Specialists (Provisioning/DC Ops/Asset/Network) | Bruce (Pending Mgr Hire)
PE (OS, firmware, SRE) |Ben
Network Architecture | Adam

__Squad Composition__

Roles| Description
:-------------| ------------- 
Product Owner (Product) | Interfaces with the business and the squad leader, determines priorities and roadmap
Tech Team leader (Software) | Translates the product into software execution plan and lead the team technically
Infra Architect | Develops the product technical design
Backend engineer (Software) | API and Microservice development
Frontend engineer (Software) | Portal work
PE | Operation tooling and automation


__Our Squads__

Squad Name    | Main Focus | SLO 
:-------------|----------- | ---  
[X-force](https://packet.atlassian.net/secure/RapidBoard.jspa?rapidView=60&useStoredSettings=true) | Customer Management and Overall Experience | [API Apdex](https://synthetics.newrelic.com/accounts/45249/monitors/ee8b6b9b-7373-411d-a801-67708572e293/sla?view=daily-sla-report) 
[Suicide Squad](https://packet.atlassian.net/secure/RapidBoard.jspa?rapidView=61&useStoredSettings=true) (SuS) | Compute Products, Provisioning | [Successful Provision % (internal)](https://northstar.packet.net/d/71i_Y0Jmz/vip-provision-metrics?orgId=1), [Customer Data Only (internal)](https://northstar.packet.net/d/RP-qZ82iz/northstar-dashboard-pusher-data-customer-only) 
[Network Warriors]() | Network Products & Automation | TBD 
[Deadlift](https://packet.atlassian.net/secure/RapidBoard.jspa?rapidView=65) | Production Engineering | [API & Network Availability]() 
[CMR](https://packet.atlassian.net/secure/RapidBoard.jspa?rapidView=66&projectKey=SWE) | Usage & Billing, Business Processes Automation | TBD

__Future Squads__

These are teams that require more focused attention but don't have the critical mass yet for a well functioning team.

Squad Name    | Main Focus | SLO | Squad Lead
:-------------|----------- | --- | -------------
[ICP]() | Asset Management (lives in SuS) | TBD | TBD
[Dev Exp]() | Building World-class APIs, scalable API/data model (in API Chapter) | TBD | TBD

### Resources

* Our [Interview](interview.md) process    
* Our [Onboarding](onboard.md) process    
* [Leading](leading.md) @ Packet and how we evaluate [performance](perf.md)    
* SWE [Overview & Roadmap](https://trello.com/b/A814D0t8/software-eng-roadmap) (private)    
* [How to create Pyschological Safety](https://hbr.org/2017/08/high-performing-teams-need-psychological-safety-heres-how-to-create-it)

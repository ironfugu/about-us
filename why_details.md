## Why we do what we do

Here are things we specifically do to help achieve our mission

__Code__

What   | Reasoning | Tooling
:------- | ----- | ---------
(Near) Atomic Changes | Pushing smaller changes allows us to deliver incremental value; also reduces chance of breakage | GitHub
High code coverage | CI is useless without good quality coverage, and we can't ship to production confidently without it | Drone
Refactor constantly | Reduce code debt on every issue you work on | GitHub, Rubocop
Branches and PRs | introduce small changes safely, ensure the code fits our philosophy, knowledge sharing | GitHub, Jira, Slack

__Docs__

What   | Reasoning | Tooling
:------- | ----- | ---------
Effective documentation | moving quickly means we work on a lot of different things, document for future teammates or yourself | GitHub Markdown, Jira, Confluence
Aligned Development | Make sure what we're working on brings business value | Trello, Jira
Knowledge Base | Make sure knowledge is shared freely | Wiki, Discourse

__DevOps__

What   | Reasoning | Tooling
:------- | ----- | ---------
Tight CI/CD | The way we can ship the code quickly and confidently | GithHub, Drone, Quay.io, Hashistack
Automated System/UI Testing | Once code is in production, is it really working?  Running things like Runscope against the API gives us confidence that new changes didn't mess up prod | Runscope
DevOps Culture| Everyone should know how stuff runs and keep an eye that services are working as expected | Rollbar, NewRelic, Hashistack

## Build something with our API

Effort Level : 2-4 hours

Your goal is to build an integration with our API.  Please review the instructions

* Pick a language
* Create a public GitHub repo and utilize any tooling you desire
* Review our [API docs](https://www.packet.com/developers/api/)
  * Understand [auth](https://www.packet.com/developers/api/#authentication)
  * Know the available [OSes](https://www.packet.com/developers/api/#operatingsystems)
  * Understand [capacity](https://www.packet.com/developers/api/#capacity)
  * [Devices](https://www.packet.com/developers/api/#devices) is the main api you'll need
* Receive an API token for this challenge
  * This will be under our "Interview" project id : ca73364c-6023-4935-9137-2132e73c20b4
  * [Tokens](https://app.packet.net/projects/ca73364c-6023-4935-9137-2132e73c20b4/settings/api-keys) will be created on a per interviewee basis (you won't have access to that link)
* Build a program that uses our API, which allows you to launch a machine and tear it down
* Provide Feedback on what you liked about this exercise as well as improvements you would make, this could be anything (from our docs to the api itself)
* Extra Credit
  * Pick any additional capabilities in our API that you'd think would be useful to add to the interface
* Upon completion, please send a link to the GitHub repo with a rough estimate on how long you took
  * If you're doing this in person, we'll walkthrough the code and feedback together
  * If you're remote, then we'll schedule a follow-up call to review it or do it in your next round of interviews

This is all on the honor system but we didn't need to tell you that ;)

### FAQ

__What is the main api endpoint?__   
`https://api.packet.net`

__Why do I get "Access denied for the current authentication token" errors accessing the `/plan` or `/facilities` api__   
The token you have is on a "project" token, so you will need to add the project info ie `/project/<id>/plan`

### What are we testing?

Read [this](https://github.com/packethost/about-us/blob/master/coding_fun.md#what-are-we-testing)

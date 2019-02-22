## Create a Page that connects to our API

Effort Level : 2-4 hours

Your goal is to build a simple page that displays data our API. Please review the instructions

* Pick a frontend framework
* Create a public GitHub repo and utilize any tooling you desire
* Review our [API docs](https://www.packet.com/developers/api/)
  * Understand [auth](https://www.packet.com/developers/api/#authentication)
  * [Devices](https://www.packet.com/developers/api/#devices) is an example api endpoint you could use
* Receive an API token for this challenge
  * This will be under our "Interview" project id : ca73364c-6023-4935-9137-2132e73c20b4
  * [Tokens](https://app.packet.net/projects/ca73364c-6023-4935-9137-2132e73c20b4/settings/api-keys) will be created on a per interviewee basis (you won't have access to that link)
* Build a simple page that uses our API
* Provide Feedback on what you liked about this exercise as well as improvements you would make, this could be anything (from our docs to the api itself)
* Upon completion, please send a link to the GitHub repo with a rough estimate on how long you took
  * If you're doing this in person, we'll walkthrough the code and feedback together
  * If you're remote, then we'll schedule a follow-up call to review it or do it in your next round of interviews

This is all on the honor system but we didn't need to tell you that ;)

### FAQ

__What is the main api endpoint?__   
`https://api.packet.net`

__Why do I get "Access denied for the current authentication token" errors accessing the `/plans` or `/facilities` api__   
The token you have is on a "project" token, so you will need to add the project info ie `/project/<id>/plans`

### What are we testing?

* Technical Acumen, can you actually code :)
* Given a consistent environment, how do you perform vs others?
* But even more importantly did you do it with the right [Core Behaviors](https://github.com/packethost/about-us#done-right-through-core-behaviors)
  * Care - Did you care to do a good job?  Did the code base pass the "sniff" test?
  * Small Steps - is your code built in an iterative way?
  * Listen, Collab - did you read the challenge carefully and ask questions when things were unclear?
  * Feedback - did you provide insightful feedback to us?
  * Seek learning - Did you explore and try different techniques for your code?  Were you able to read the instructions and fill in the gaps independently?

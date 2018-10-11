## Our Interview Process

* Have desire to work for us or got a warm intro from an fellow Packeteer
 * Carefully read our [dev culture](dev_culture.md) doc
* Initial HR Phone Screen
* Send us your Bam (Be a Mentor) / Sams (Seek a mentor) YAML file (using your GitHub handle as the name)
* Initial Tech Screen - casual convo about your past experience
* Onsite Process - This would typically be an entire day at our NYC or Palo Alto office
    * Interview 1 : With a peer or two on your Bam (1 hour)
    * Interview 2 : With a mentee or two on your Bam (1 hour)
    * Interview 3 : With a mentor or two on your Sam (1 hour)
    * Lunch : Casual chat with some team members (1 hour)
    * Tech Screen : 2-4 hours talking about the right challenge
* Remote Process - This process may span a week, but ideally it would be within a week
    * Zoom Interview 1 : With a peer or two on your Bam
    * Zoom Interview 2 : With a mentee or two on your Bam
    * Zoom Interview 3 : With a mentor or two on your sam
    * Tech Challenge : Select a task and have up to a week to complete
    * Zoom Executive Interview - With CTO or CEO
* Executive Interview - With CTO or CEO

More details are in our private [trello](https://trello.com/b/pVJcxCm6/software-hiring) board.

## Tech/Coding Challenges

Most of these should be doable in 3-4 hours of time.  If the person is remote, I think we can try to give tasks that could span 1-2 days.

### Improve our API / Refactoring

Level : Seniorn    
Time : 4 - 8 hours   
Type : Backend   

* Login to our [NewRelic account](https://rpm.newrelic.com/accounts/45249/applications/9068939)
 * Provide 3 areas of suggestions for the code base
 * Out of the 3, pick one area which you'd like to explore
* Provide the candidate a "redacted" version of our API code base
* Issue PR for refactor of the "trouble" area

### Break the monolith

Level : Senior   
Time : 8-16 hours   
Type : Backend   

* Provide a "redacted" version of our API code base
* Review the code base and decide what areas would you suggest to refactor and to break up into several "macro-services".  Below are areas to review
 * Our `app/jobs/` directory
 * Our `lib/` directory
 * Our `spec` directory
 * Our `routes.rb` file

### Improve our SDKs

Level : Any   
Time : 2-4 hours   
Type : Backend   

* Pick a language (that we have a SDK for)
* Review the SDK and then make changes to it and issue a PR
* The interviewer will do a code review with the person and walk through the changes

### Be a customer

Level : Any   
Time : 2-4 hours   
Type : Backend   

* Provider person with a dev account.
* Use our API / SDKs / Getting started guide to launch a small farm of machines to run a frontend/backend "hello world" app.
 * The front end should display a message
 * THe backend API should provide the response that the front-end should display, start with "Hello World"

### Improve our UI

Level : Any   
Time : 2-4 hours   
Type : Frontend   

* Login to Rollbar and review our staff portal [exceptions](https://rollbar.com/Packet/Staff-Portal/)
* Pick one of the exceptions to [debug](https://rollbar.com/Packet/Staff-Portal/items/2414/)
* Provide access to our Staff Portal code base
* Debug on what you think the problem is

### Script to review our bam/sams

Level : Any   
Time : 4-8 hours   
Type : Backend   

* Create a program to review our "employees" and "candidates" yml file and decide how to match up people for interviews.  Match up 1 or 2 employyes who are:
 * are "bams" peers to the candidate
 * are "sams" to the candidate
 * are "bams" to the candidate's sam
* It should output an interview schedule and highlight what the match citeria was on to help focus the interview
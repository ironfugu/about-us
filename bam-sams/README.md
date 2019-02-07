## Be a mentor / Seek a mentor (Bam/Sams)

The concept of a bam/sam is to what we consider a more modern and dynamic version of a "resume".  It also fits with our core beavhior of "seek learning, be uncomfortable".  We want to encourge a culture of mentorship where we can learn from each other and find ways to grow our skills.  We take this bam/sam, and then create both an on-boarding guide based on that, as well as a personal development plan to grow your skills and capabilities.  For candidates and employees alike, we store this info in a private repo but you can see the examples below, along with some examples.

Let's take a closer look at our template.yml

### Overview

There are 3 main sections, an "about", "bam" and "sam".  You can see the details below.

```json
about:
  name: Packet Bot
  location: The Internets
  timezone: UTC-00
  hobbies:
    - "Ultimate Frisbee"
  favorite_resources:
    - "ai superpowers"
# be a mentor
bam:
  skills:
    - Breaking stuff
    - Being Awesome
    - Making the internet a better place
  languages/paradigms:
    # Specify ["what", 1], level 1-10 (1 being justed learned, 10 you wrote/contributed to the language)
    - ["RocketLang", 10]
    - ["Go", 9]
    - ["Ruby", 8]
  frameworks/libraries/concepts:
    # list in order of most recent
    - None
# seek a mentor
sam:
  skills:
    - Letting others have their sunshine
    - Edge Computing
    - Datacenter Monitoring
  languages/paradigms:
    - Rust
  frameworks/libraries/concepts:
    - React
```

### Onboarding

This section is created by your manager before you start at Packet.  The idea here is to have a clear onboarding plan, and how you can get ramped up but also contribute to Packet quickly.

```json
# The onboarding plan is created when you join
onboarding:
  sam_to_bam: "Learn react"
  bam: "Help interns learn about Golang"
  # your manager will help fill this out with you to determine the best use of your time to get onboarded quickly
  # and contributing to the team quickly
  week:
    - "Take a udacity course about Advanced AI"
  month:
    - "Run algorithms on GCP and Azure"
  quarter:
    - "Present at IEEE"
  # list a person inside or outside the company who can help you achieve your plan
  mentor: "Dave"

```

### Personal Development Plan (PDP)

PDP is created after you initial evlauation period, or our yearly career discussions (which we check up on quarterly.  Note that the updates will be handled through Lattice.

```json
# Personal Development plan, created during your career discussions or your evaluation period after your start date
pdp:
  # career goal.  Additional improvements to help your career
  goals:
    career: "I can turn off an entire datacenter and survive"
    sam_to_bam: "Datacenter monitoring"
    bam: "Build out Go foundational libraries"
  # list at least 2 things Packet can be doing to help
  support:
    - "Run me on bigger hardware"
    - "Attend machine learning courses"
  # your plan will be created in Lattice and updates can be made there.  It will take an "OKR" type format
  ```

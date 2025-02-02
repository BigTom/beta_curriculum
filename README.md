# Beta Academy Curriculum
To open the .livemd files you will need the latest version of [livebook](https://github.com/livebook-dev/livebook) running.

We use some experimental features so ensure you install livebook main.

```
mix escript.install github livebook-dev/livebook
```

Click on the `instructions.livemd` file while running livebook. Then click the "Open" button nearby.
From here, you'll be able to follow the links to access each lesson and exercise.

## Getting Started
- Ensure you have [asdf](https://asdf-vm.com/guide/getting-started.html#_1-install-dependencies) installed or a compatable local Elixir version as found in `.tool-versions`.
- Ensure you have the latest [livebook](https://github.com/livebook-dev/livebook) installed.
- Run the project with `livebook server`.
- Go to the `instructions.livemd` to see the course content.

It's common for incorrect versions to cause an issue where mermaid graphs cannot be displayed.

## Philosophy
The academy follows a flipped classroom design where students complete interactive instructional material,
and then perform exercises and create projects inspired by the learning material.

The academy is inspired by:
- Scaffolded Design
- Backwards Design
- Collaborative Learning
- Flipped Classroom Design
- Intrinsic Motivation
- Dreyfus Model of Skill Acquisition

## Class time

Instruction will focus on supporting student exercises rather than lecture.

Class time will be broken into
1. **Assessment & Review**
1. **Exercises**
1. **Labs**
1. **Support & Self-Instruction Time**

### Assessment & Review
Assessment will provide the teacher an understanding of how students incorporated the learning from the
previous interactive instruction, and will provide reactive lectures based on what students require more
instruction in. Review will provide the students an opportunity to recall prior information and review
any topics that require it.

### Exercises
Exercises will provide students an opportunity to practice drilled repetition and reinforce the prior interactive
instruction. Exercises should be concrete, repeatable drills. Exercises should build upon established topics. 

### Labs
Labs will challenge students to combine the concepts drilled during the exercise phase at a higher level. Labs have a wider variety of solutions and are expected to push students beyond the knowledge they learned in class. Students will need to assess how to solve the problem using the knowledge and tools learned prior. Students may also need to do additional research and learn concepts beyond those taught in class.

### Midterm Group Project
Students will complete a group project that will teach them how to work effectively as a team.

### Capstone Project
Students will complete a capstone project that incorporates the skills they have learned so far from the academy.
This will serve to give them experience working on a larger project and managing time pressure and complexity.

### Grading
Students will not receive a number or letter grade for this course. Due to the nature of the assignments,
this course will be completion-based and rely on the intrinsic motivation of learning and self-improvement rather than
carrot and stick motivation.

For more on this see [Mark Rober's Talk](https://www.youtube.com/watch?v=9vJRopau0g0&ab_channel=TEDxTalks).

## Class Culture & Values
Class values will be reinforced continuously to students.
- Rely On Your Cohort. Support Each Other.
- Failure Is Ok. I.E. "Red Is The First Step."
- Get Ahead, Don't Fall Behind.
- Attend Support Time And Help Others.
- Turn On Your Cameras If Possible.

## Student Goals
Students will be competent developers prepared to excel in the Elixir industry. They will have
a solid grasp of Elixir fundamentals, Elixir project development, Phoenix project development, and OTP.
They will also have the researching and problem-solving skills necessary to expand their skill set and thrive
throughout their career. Students will be capable of delivering high-quality, well-tested features to a production complexity codebase.

## Writing Guide

- Code keywords such as `defimpl`, `defprotocol`, and `end` should use backticks (``).
- Important or new concepts should be in **bold** the first time you introduce them.
- Use title case without a period in headers.
- Code should be in an executable elixir cell unless it is pseudocode or it reduces the clarity of the lesson.
- Text should be run through [grammarly](https://app.grammarly.com/) to ensure correctness. The free features should be sufficient.
- Lessons should have a `Setup` section for any necessary dependencies.
- Each new major concept should be in its own section. Each section should strive to provide at least one student interaction portion, typically using the **Your Turn** heading.

## Curriculum Outline
The curriculum is still a rough outline subject to change and feedback.

The course is broken into 5 major sections:
1. Getting Started
2. Fundamentals
3. Elixir Project Development
4. Phoenix Project Development
5. OTP

### Getting Started
- Why Elixir?
- Why Functional Programming?
- Course Outline
- Communication Tools
- Development Environment
  - Using the Terminal
    - mkdir
    - cd
    - rm
    - ls
    - mv
    - env variables
      - export
    - $PATH
      - hello - command not found, what's it trying to do?
      - elixir - finds it - where did it find it and why?
      - add something to the path
  - Windows Users: WSL
  - Install Git & SSH (Terminal or GitHub Desktop TBD)
  - Install Visual Studio Code and Extensions
    - ElixirLS
    - WSL: Remote Development Pack
    - Optional: Elixir Testing & Other Useful Recommendations.
  - Using Visual Studio Code LiveShare to Collaborate
  - asdf (may be able to wait for elixir dev section)
    - plugins
    - .tool-versions
  - hex
- Run the Curriculum Repo
  - Clone the Repo
  - Install & Configure Postgres
  - Install Elixir & Erlang
  - May need to install inotify tools
  - Install & Run Livebook
  - Run Local Tests
- Livebook & Lesson Guide
  - Example Lesson Outline
    - Overview
    - Setup
    - Sections
    - Markdown Cells
    - Elixir Cells
    - Answering Questions with `=`
    - Evaluating Cells
  - How to Recover From Accidental Deletion
  - Running Tests
  - Using Kino Inputs

### Fundamentals
- Data Types
  - Comments 
  - Data and Variables
  - Integers
  - Floats
  - Strings
  - Atoms
  - Booleans
  - Lists
  - Ranges
  - Tuples
  - Keyword Lists
  - Maps
- Operators
  - Variables
  - Arithmetic (+, -, /, *, rem, div)
  - Strings (<>)
  - Comparison Operators (===, ==, <=, >=, >, <)
  - List Manipulation (++, --)
  - Boolean Operators (and, or, not)
  - (||, &&, !)
  - Sorting order number, atom, reference, function, port, pid, tuple, map, list, bitstring
  - Accessing Map Values map[:a]
- Modules and Functions
  - Abstracting & Repeating Behavior
  - First Class Functions
  - Arity
  - Module Definition
  - Public vs Private Functions
  - Module Attributes
  - Pipe Operator: Small Composable Functions. One Responsibility.
  - Common Modules
    - Date & Time
    - Map Module
    - String Module
    - List Module
    - Tuple Module
    - Keyword Module
  - Structs
  - Behaviors
  - Protocols
- Control Flow
  - If & Unless
  - Case
  - Cond
  - Pattern Matching
  - With
  - Multi-clause Functions
  - Guards
  - Error Handling
- Enumeration
  - Collections
  - Linked List + Stack and Heap.
  - Tail-call Optimization
  - Enum
  - Comprehensions
  - Recursion
  - Streams
- Erlang Interoperability
  - What is Erlang?
  - Using Tools from Erlang
    - :rand
    - :timer
    - :ets
    - :math
  - The Erlang Standard Library
    - https://www.erlang.org/doc/apps/stdlib/
    - https://elixir-lang.org/getting-started/erlang-libraries.html
- Ecto
  - Persistence
  - File Based DB and Problems
  - Query
  - What is a Database?

### Elixir Development
- Intro to Elixir
  - Interactive Shell IEX
    - Autocomplete
    - h
  - Running Scripts
  - Print Debugging with IO
  - use, import, require, alias
- Mix
  - Using Git and GitHub
  - ASDF
  - New Project
  - Project Structure
  - Compiling Project + Compiled vs Interpreted Languages
  - Mix Tasks
  - Dialyzer, Specification and Types
  - Code Formatting
  - Credo
  - Libraries & Dependencies
  - Using IEX in a Project
- Communicative Code (Clarity) (Where does this section belong?)
  - Dichotomy (Tests too DRY)
  - Writing For Your Future Self and Teammates
    - Criteria: Do We Understand The Code Well Enough To Work On It.
  - Refactoring? (Showing examples of poor code and contrasting with examples of good code)
  - Verbose Variable Names
  - Explicit Function Names
- Documentation & Testing
  - Running Tests
  - Annotation
  - ExDoc: Generate Documentation
  - How to Find and Read Online Documentation with HexDocs
  - Doc Testing
  - Testing with ExUnit
    - Assert Message, Interpolation
    - What Do I Want The Test To Tell Me?
  - 3As of Testing
  - TDD + Spike
  - Error Handling
    - Match Errors
    - Custom Error Structs
- APIs and External Dependencies
  - API Fundamentals
    - What is a Web Server?
    - What is an API?
    - What is REST?
    - JSON
    - What is GraphQL? 
    - What is CRUD?
    - What is a Database?
  - Calling an API
  - Calling a GraphQL API
  - Calling an API with Authentication
- Debugging Tools & Techniques
  - Reading Errors
  - IEx.pry
  - :debugger and :int https://elixir-lang.org/getting-started/debugging.html#iexpry0-and-iexbreak2
  - How to Debug Crashes
  - Compile Time vs Runtime bugs
  - Common Causes of Bugs
    - Time & Timing
    - Incorrect Logic
    - State & Data
    - Syntax Errors
- Intro to Concurrency, OTP, Erlang, and the BEAM
  - Fault Tolerance, Scalability, Distribution, Responsiveness
  - What is a Process?
  - BEAM VM & Scheduler
    - OS Threads & Lightweight BEAM Processes
    - Execution Window (Reductions) & Non-Blocking Execution
    - Shared-nothing Concurrency & Garbage Collection
  - Parallel vs Concurrent
  - Understanding Generic Server Processes (Genservers)
    - Stateful Server Processes
    - Message Passing: https://elixirschool.com/en/lessons/advanced/otp_distribution
    - Point of Synchronization
    - Process Mailbox
    - Generic Server Process Lifecycle
    - Custom Genserver
    - Exercise: Sending Messages Back And Forth
  - Use Genserver Basics
    - start_link, init, cast, call, info
    - Client/Server API
    - pids
    - Singletons
  - Agent & Task
  - Understanding Supervisors
    - Supervision Trees
    - Running a Project in a Supervisor
      - mix new project --sup

### Phoenix Web Development
- What is the Phoenix Framework?
  - How Phoenix Leverages OTP
  - MVC Architecture (Checking with Chris)
  - New Phoenix Project
  - Phoenix Project Structure: Endpoint, Router, Controller, View, Template, Context, Repo, Schema, Migration
  - Sigils (In Context of Templates)
- Phoenix Generators
- ECTO
  - Relational DBs
    - Associations
    - Tables
- Phoenix Templates: HTML & CSS
  - Common HTML Elements
  - Box Model
  - Basic Syntax & Formatting
  - Recreating Styles
  - Tailwind
  - Alpine JS
- Phoenix Authentication
- Phoenix LiveView
- PubSub
- Channels
- GraphQL & Absynth
- Umbrella Projects
- Live Dashboard & Monitoring
- Deployment with Releases (Cuttable?)

### OTP & Concurrency
- Genservers
  - Bottlenecks
  - Worker Pools
  - Registration (Singletons vs Worker vs Pool)
  - Testing: https://www.youtube.com/results?search_query=architecting+genservers+for+testability&ab_channel=ElixirConf
  - Debugging with :sys
- Supervisors
  - Restart Strategies
  - Dynamic Supervisor
  - Task Supervisor
- ETS

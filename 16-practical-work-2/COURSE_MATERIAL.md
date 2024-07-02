[markdown]:
  https://github.com/heig-vd-dai-course/heig-vd-dai-course/blob/main/16-practical-work-2/COURSE_MATERIAL.md
[pdf]:
  https://heig-vd-dai-course.github.io/heig-vd-dai-course/16-practical-work-2/16-practical-work-2-course-material.pdf
[license]:
  https://github.com/heig-vd-dai-course/heig-vd-dai-course/blob/main/LICENSE.md
[discussions]: https://github.com/orgs/heig-vd-dai-course/discussions/117
[illustration]:
  https://images.unsplash.com/photo-1610633389918-7d5b62977dc3?fit=crop&h=720

# Practical work 2

<https://github.com/heig-vd-dai-course>

[Markdown][markdown] · [PDF][pdf]

L. Delafontaine and H. Louis, with the help of Copilot.

This work is licensed under the [CC BY-SA 4.0][license] license.

![Main illustration][illustration]

## Table of contents

- [Table of contents](#table-of-contents)
- [Introduction](#introduction)
- [Objectives](#objectives)
- [Group composition](#group-composition)
- [Grading criteria](#grading-criteria)
  - [Category 1 - Git, GitHub and Markdown](#category-1---git-github-and-markdown)
  - [Category 2 - Java, IntelliJ IDEA and Maven](#category-2---java-intellij-idea-and-maven)
  - [Category 3 - Define an application protocol](#category-3---define-an-application-protocol)
  - [Category 4 - Java TCP programming](#category-4---java-tcp-programming)
  - [Category 5 - Presentation and questions](#category-5---presentation-and-questions)
- [Constraints](#constraints)
- [Remarks](#remarks)
- [Submission](#submission)
- [Grades and feedback](#grades-and-feedback)
- [Finished? Was it easy? Was it hard?](#finished-was-it-easy-was-it-hard)
- [Sources](#sources)

## Introduction

Network applications are everywhere. They are used to communicate, to play
games, to watch videos, to listen to music, to browse the web, to send emails,
etc.

In this practical work, you will create a network application that uses the TCP
protocol.

The network application will be defined by an application protocol, a client and
a server. The client will send some requests to the server and the server will
send some responses to the client.

The application protocol will be defined by you.

Feel free to be creative! For example, you can choose to create a chat
application, a chess game, a shopping list, etc. If you do not have any idea,
come to see us and we can give you.

Multiple groups can choose the same application protocol and you can share your
methodology but please do not copy/paste code from other groups.

## Objectives

- Define a network application protocol
- Make usage of the TCP protocol
- Use Java TCP programming to implement a client and a server application

## Group composition

You will work in groups of two students. You can choose your partner. If you do
not have a partner, we will assign you one.

To announce your group, create a new GitHub Discussion at
<https://github.com/orgs/heig-vd-dai-course/discussions> with the following
information:

- **Title**: DAI 2023-2024 - Practical work 2 - First name Last name member 1
  and First name Last name member 2
- **Category**: Show and tell
- **Description**: A quick description of what you will achieve during this
  practical work

The teaching staff might ask you to change the scope of your practical work if
it is too complex or too simple.

**Please do it a soon as possible, even if you do not have a clear idea yet as
it will help us to plan the practical work review.**

## Grading criteria

- 0 point - The work is not done
- 0.1 point - The work is insufficient
- 0.2 point - The work is done

Maximum grade: 25 points \* 0.2 + 1 = 6

### Category 1 - Git, GitHub and Markdown

If your repository is private, you must add us as collaborators to your
repository!

| #   | Criterion                                                                                                               | Points |
| --- | ----------------------------------------------------------------------------------------------------------------------- | -----: |
| 1   | The whole team contributes to the project and can explain it in details                                                 |    0.2 |
| 2   | The README is well structured and explains what the network application is for with its documented application protocol |    0.2 |
| 3   | The README explains how to build the network application                                                                |    0.2 |
| 4   | The README explains how to run the network application with examples and outputs                                        |    0.2 |

### Category 2 - Java, IntelliJ IDEA and Maven

| #   | Criterion                                                  | Points |
| --- | ---------------------------------------------------------- | -----: |
| 5   | The codebase has all required files and is well structured |    0.2 |
| 6   | The codebase is well documented                            |    0.2 |

### Category 3 - Define an application protocol

| #   | Criterion                                                                                     | Points |
| --- | --------------------------------------------------------------------------------------------- | -----: |
| 7   | The application protocol defines the port and protocol to use                                 |    0.2 |
| 8   | The application protocol defines who initiates the connection and how                         |    0.2 |
| 9   | The application protocol defines the available messages/actions with their input(s)/output(s) |    0.2 |
| 10  | The application protocol defines the success/error codes and their explanations               |    0.2 |
| 11  | The application protocol is described using one or multiple diagrams                          |    0.2 |
| 12  | The application protocol defines the edge-cases when something could go wrong with a diagram  |    0.2 |

### Category 4 - Java TCP programming

| #   | Criterion                                                                                                                                                                                                                                                                    | Points |
| --- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -----: |
| 13  | The server starts on the defined port (but you must be able to change it if needed) and accept connections from multiple clients at the same time                                                                                                                            |    0.2 |
| 14  | The client can access the server on a given host (by default, the client tries to connect to the defined port but you must be able to change it if needed) and execute commands to interact with it without closing the connection for each action (see [Remarks](#remarks)) |    0.2 |
| 15  | The client displays an error message with details when the connection has not succeed                                                                                                                                                                                        |    0.2 |
| 16  | Some actions are private (unique to one user), some actions are common (affect all users)                                                                                                                                                                                    |    0.2 |
| 17  | No one can manipulate items from another client if it is not authorized                                                                                                                                                                                                      |    0.2 |
| 18  | The client and server correctly process the input/output commands                                                                                                                                                                                                            |    0.2 |
| 19  | The client/server is informed if the server/client closes the connection                                                                                                                                                                                                     |    0.2 |
| 20  | The application uses all the best practices regarding network programming                                                                                                                                                                                                    |    0.2 |

### Category 5 - Presentation and questions

| #   | Criterion                                                                            | Points |
| --- | ------------------------------------------------------------------------------------ | -----: |
| 21  | The presentation is clear and well prepared                                          |    0.2 |
| 22  | Everyone speaks during the presentation, and the presentation lasts the time allowed |    0.2 |
| 23  | The presentation presents the network application                                    |    0.2 |
| 24  | A demo of the network application is made                                            |    0.2 |
| 25  | The answers to the questions are correct                                             |    0.2 |

## Constraints

- The network application must be written in Java, compatible with Java 17
- The network application must be built using Maven
- You must use one or more of the Java classes seen in the course
- Your application must be slightly more complex and different than the ones
  presented during the course

## Remarks

Remember the KISS principle: Keep It Simple, Silly! Sometimes it is better to
use a simple solution than a complex one.

If your implementation is too complex, we might penalize you.

If elements that are supposed to be acquired through the course or previous
practical works are omitted, forgotten or poorly implemented, we might penalize
you.

You can use [PlantUML](https://plantuml.com/), [Draw.io](https://draw.io/) or
any other tools you want to create your diagrams.

You can use any other dependencies you want in your Maven project. You must
however explain why and how you use it in your README.

You can protect the `main` branch of your repository to prevent any push on it
and force signed commits from team members. This will force all team members to
use signed pull requests to merge your work.

In order to run multiple commands/actions on the server without closing the
connection, you can use what is called a
[read-eval-print loop (REPL)](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop).
To make it simple, a REPL is simply a loop that will ask the user to input
commands. The loop will then execute the command and display the result. The
loop will continue until the user decides to exit the loop.

## Submission

Your work is due on the **day of the presentations** (the _"Practical work
review"_ sessions in the official planning available at
<https://github.com/orgs/heig-vd-dai-course/projects>) at **13:15**.

Any commit after the deadline will not be taken into account. Each day of delay
will result in a penalty of -1 point on the final grade.

You must update the GitHub Discussion you created previously with the following
information:

- **Description**: The link to your repository as well as the latest commit hash
  of your work before submission

## Grades and feedback

Grades will be entered into GAPS, followed by an email with the feedback.

The evaluation will use exactly the same grading grid as shown in the course
material.

Each criterion will be accompanied by a comment explaining the points obtained,
a general comment on your work and the final grade.

If you have any questions about the evaluation, you can contact us!

<details>
<summary>Grading grid template for the teaching staff</summary>

```markdown
# Practical work 2 - Grading grid for First name Last name member 1 and First name Last name member 2

Here are the grades and comments for each criterion for the practical work.

## Grading criteria

- 0 point - The work is not done
- 0.1 point - The work is insufficient
- 0.2 point - The work is done

Maximum grade: 25 points \* 0.2 + 1 = 6

## General feedback

- ...

## Final grade

Your final grade is:

Feel free to contact us if you have any questions about the evaluation!
```

</details>

## Finished? Was it easy? Was it hard?

Can you let us know what was easy and what was difficult for you during this
practical work?

This will help us to improve the course and adapt the content to your needs. If
we notice some difficulties, we will come back to you to help you.

➡️ [GitHub Discussions][discussions]

You can use reactions to express your opinion on a comment!

## Sources

- Main illustration by [Rafael Rex Felisilda](https://unsplash.com/@rafaelrex)
  on
  [Unsplash](https://unsplash.com/photos/chess-pieces-on-chess-board-rCxTJlaU5Yc)

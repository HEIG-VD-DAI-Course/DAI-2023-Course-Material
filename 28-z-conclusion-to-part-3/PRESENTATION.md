---
marp: true
---

<!--
theme: gaia
size: 16:9
paginate: true
author: L. Delafontaine and H. Louis, with the help of ChatGPT
title: 'HEIG-VD DAI Course - Conclusion to part 3: Network programming with UDP'
description: 'Conclusion to part 3: Network programming with UDP for the DAI course at HEIG-VD, Switzerland'
url: https://heig-vd-dai-course.github.io/heig-vd-dai-course/19-conclusion-to-part-3/
footer: '**HEIG-VD** - DAI Course 2023-2024 - CC BY-SA 4.0'
style: |
    :root {
        --color-background: #fff;
        --color-foreground: #333;
        --color-highlight: #f96;
        --color-dimmed: #888;
        --color-headings: #7d8ca3;
    }
    blockquote {
        font-style: italic;
    }
    table {
        width: 100%;
    }
    th:first-child {
        width: 15%;
    }
    h1, h2, h3, h4, h5, h6 {
        color: var(--color-headings);
    }
    h2, h3, h4, h5, h6 {
        font-size: 1.5rem;
    }
    h1 a:link, h2 a:link, h3 a:link, h4 a:link, h5 a:link, h6 a:link {
        text-decoration: none;
    }
    section:not([class=lead]) > p, blockquote {
        text-align: justify;
    }
headingDivider: 4
-->

[web]:
  https://heig-vd-dai-course.github.io/heig-vd-dai-course/19-conclusion-to-part-3/
[pdf]:
  https://heig-vd-dai-course.github.io/heig-vd-dai-course/19-conclusion-to-part-3/19-conclusion-to-part-3-presentation.pdf
[license]:
  https://github.com/heig-vd-dai-course/heig-vd-dai-course/blob/main/LICENSE.md
[feedback]: https://framaforms.org/dai-2023-2024-feedback-3-1700494438
[feedback-qr-code]:
  https://quickchart.io/qr?format=png&ecLevel=Q&size=400&margin=1&text=https://framaforms.org/dai-2023-2024-feedback-3-1700494438
[illustration]:
  https://images.unsplash.com/photo-1631220706319-657942774d02?fit=crop&h=720

# Conclusion to part 3: Network programming with UDP

<!--
_class: lead
_paginate: false
-->

<https://github.com/heig-vd-dai-course>

[Web][web] · [PDF][pdf]

<small>L. Delafontaine and H. Louis, with the help of ChatGPT.</small>

<small>This work is licensed under the [CC BY-SA 4.0][license] license.</small>

![bg opacity:0.1][illustration]

## What have you learned?

- Network programming with UDP with all its elements:
  - Reliability
  - Unicast, broadcast and multicast
  - Messaging patterns
  - Service discovery protocols
- The differences between TCP and UDP

![bg right:40%](https://images.unsplash.com/photo-1549228581-cdbdb7430548?fit=crop&h=720)

## What have you accomplished?

- You have implemented an UDP application in Java with some concurrency patterns
  (for some)
- You have defined your own application protocol (again, yeah!)
- Deeper usage of Docker and Docker Compose to build, share and run your network
  application

![bg right:40%](https://images.unsplash.com/photo-1608613304810-2d4dd52511a2?fit=crop&h=720)

## Evaluation

In order to validate this part of the course, you will have to pass an
evaluation. The questions will be in French and you can answer them in French or
English.

The evaluation will only be **a theoretical part of 60 minutes**.

The evaluation will be done on the computer with the help the online evaluation
platform as used in the evaluation 1.

You will have to be connected to the
[VPN](https://intranet.heig-vd.ch/services/informatique/poste-de-travail/reseau/vpn/Pages/vpn.aspx).
It is **mandatory**.

---

The following chapters will be evaluated:

- [Define an application protocol](https://github.com/heig-vd-dai-course/heig-vd-dai-course/tree/main/11-define-an-application-protocol)
- [Docker and Docker Compose](https://github.com/heig-vd-dai-course/heig-vd-dai-course/tree/main/06-docker-and-docker-compose)
- [Java UDP programming](https://github.com/heig-vd-dai-course/heig-vd-dai-course/tree/main/14-java-udp-programming)

---

You might be asked questions about the theoretical content, the practical
content and elements seen in the practical work.

You can only have access to your own notes in paper format. Your notes must fit
on one sheet of paper (recto). They can contain anything useful to you:
definitions, schemas, code snippets, etc. You will be able to use them during
the exam at the end of the semester.

All typical questions are at the end of each chapter you studied.

All previous evaluations are available in the
[`evaluation-and-exam-archives`](https://github.com/heig-vd-dai-course/heig-vd-dai-course/tree/main/00-evaluation-and-exam-archives)
folder of the course repository.

## Questions

<!-- _class: lead -->

Do you have any questions?

## Feedback

Your feedback helps us know **what what you liked and what you disliked** in
your learning experience. **The feedback is anonymous**.

We would be very grateful if you could [take a few minutes to fill
it][feedback]. **Thank you!**

[![bg right w:75%][feedback-qr-code]][feedback]

## Sources

- Main illustration by [Allie Reefer](https://unsplash.com/@thepghtraveler) on
  [Unsplash](https://unsplash.com/photos/rAoQn6kwv64)
- Illustration by [Nils Stahl](https://unsplash.com/@nilsjakob) on
  [Unsplash](https://unsplash.com/photos/neUbjUnjXNk)
- Illustration by [Samantha Fortney](https://unsplash.com/@goldencoastgrams) on
  [Unsplash](https://unsplash.com/photos/OGDyzpsTjyA)

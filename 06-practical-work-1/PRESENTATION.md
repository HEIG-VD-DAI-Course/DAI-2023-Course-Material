---
marp: true
---

<!--
theme: gaia
size: 16:9
paginate: true
author: L. Delafontaine and H. Louis, with the help of ChatGPT
title: HEIG-VD DAI Course - Practical work 1
description: Practical work 1 for the DAI course at HEIG-VD, Switzerland
url: https://heig-vd-dai-course.github.io/heig-vd-dai-course/06-practical-work-1/
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
  https://heig-vd-dai-course.github.io/heig-vd-dai-course/06-practical-work-1/
[pdf]:
  https://heig-vd-dai-course.github.io/heig-vd-dai-course/06-practical-work-1/06-practical-work-1-presentation.pdf
[license]:
  https://github.com/heig-vd-dai-course/heig-vd-dai-course/blob/main/LICENSE.md
[discussions]: https://github.com/orgs/heig-vd-dai-course/discussions/5
[illustration]:
  https://images.unsplash.com/photo-1583736902935-6b52b2b2359e?fit=crop&h=720
[practical-work]:
  https://github.com/heig-vd-dai-course/heig-vd-dai-course/blob/main/06-practical-work-1/COURSE_MATERIAL.md
[practical-work-qr-code]:
  https://quickchart.io/qr?format=png&ecLevel=Q&size=400&margin=1&text=https://github.com/heig-vd-dai-course/heig-vd-dai-course/blob/main/06-practical-work-1/COURSE_MATERIAL.md

# Practical work 1

<!--
_class: lead
_paginate: false
-->

<https://github.com/heig-vd-dai-course>

[Web][web] · [PDF][pdf]

<small>L. Delafontaine and H. Louis, with the help of ChatGPT.</small>

<small>This work is licensed under the [CC BY-SA 4.0][license] license.</small>

![bg opacity:0.1][illustration]

## Practical work 1

- A CLI to process files
- Use Java, Maven and [picocli](https://picocli.info/)
- You can choose what the CLI will do (you can be creative!)
  - Transform the input file to lowercase/uppercase, convert a PNG to JPEG, ...
- Publish your CLI on GitHub

![bg right:40%][illustration]

## Demo

- Compile the project

```sh
mvn clean package
```

- Run the CLI without any arguments

```sh
java -jar target/practical-work-1-demo-1.0-SNAPSHOT.jar
```

---

```sh
Missing required options: '--input=<inputFile>', '--output=<outputFile>'
Usage: IoProcessing [-hV] -i=<inputFile> [-ie=<inputEncoding>] -o=<outputFile>
                    [-oe=<outputEncoding>] [COMMAND]
Process an input file and return a result.
  -h, --help                Show this help message and exit.
  -i, --input=<inputFile>   The input file.
      -ie, --input-encoding=<inputEncoding>
                            The input file encoding.
  -o, --output=<outputFile> The output file.
      -oe, --output-encoding=<outputEncoding>
                            The output file encoding.
  -V, --version             Print version information and exit.
Commands:
  uppercase  Converts the input file to uppercase.
  lowercase  Converts the input file to lowercase.
```

---

- Run the CLI with the `uppercase` command

```sh
java -jar target/practical-work-1-demo-1.0-SNAPSHOT.jar -i input.txt -o output.txt uppercase
```

- You can also specify the encoding of the input and output files

```sh
java -jar target/practical-work-1-demo-1.0-SNAPSHOT.jar \
    -i input.txt -ie UTF-8 \
    -o output.txt -oe US-ASCII uppercase
```

## See the result

```sh
$> cat input.txt
Coucou ça va ?
```

```sh
$> cat output.txt
COUCOU ?A VA ?
```

Why is the `ç` not converted to uppercase?

## Find the practical work

<!-- _class: lead -->

You can find the practical work for this part on [GitHub][practical-work].

[![bg right w:75%][practical-work-qr-code]][practical-work]

## Grades and feedback

Grades will be entered into GAPS, followed by an email with the feedback.

The evaluation will use exactly the same grading grid as shown in the course
material.

Each criterion will be accompanied by a comment explaining the points obtained,
a general comment on your work and the final grade.

If you have any questions about the evaluation, you can contact us!

## Finished? Was it easy? Was it hard?

Can you let us know what was easy and what was difficult for you during this
practical work?

This will help us to improve the course and adapt the content to your needs. If
we notice some difficulties, we will come back to you to help you.

➡️ [GitHub Discussions][discussions]

You can use reactions to express your opinion on a comment!

## Sources

- Main illustration by
  [Birmingham Museums Trust](https://unsplash.com/@birminghammuseumstrust) on
  [Unsplash](https://unsplash.com/photos/ScZwMqoxcls)

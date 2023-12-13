# FCEWebsite.github.io

# Design Detailed Document (DDD)

## Project Title
My first website (Practical work II (FCE))

---
## Table of Contents
1. [Introduction](#introduction)
2. [Description of the Work](#description-of-the-work)
3. [Problems Faced](#problems-faced)
4. [Conclusions](#conclusions)
5. [Additional Sections (if any)](#additional-sections)

---
## Introduction
This project consists on creating a website using HTML (HyperText Markup Language) and CSS (Cascaded Style Sheets) combining their characteristics and using certain layout and style techniques to create the best website possible.

The aim of this project is to gain knowledge about the programming languages used to make the front-end of most web pages and to understand how most of the characteristics of web pages are displayed by web browsers and expressed in these languages.

---
## Description of the Work
The website was created through the use of HTML and CSS in Visual Studio Code (Msft) and a distributed source code repository using GitHub.

The actual developement of the source code of the website took place in the local directory and, when finished, uploaded to the remote repository. This upload created some issues which are described below.

### Key Features
This website contains 7 webpages:

#### Home (index.html)
Contains basic information and links to all the other web pages.

#### About me (about.html)

Contains information about the developer of the practical work. Includes:

- Basic infomration about the developer (me, Marcos García Balboa)
- A downloadable curriculum vitae pdf.

#### IoT (topic.html)
Contains information about the researched topic in practical work I. In this case, the Internet of Things (IoT). Includes:

- The IoT technology
- How is IoT possible?
- IoT applications
- Advantages and diadvantages of IoT
- The future of IoT
- The ethical view
- Conclusions
- A downloadable pptx about IoT

#### Net (net.html)
Contains links to other partners' websites

#### Degree (degree.html)
Contains information about the Business Analytics + Computer Engineering degree. Includes

- A description of all the subjects in year 2023/2024 grouped by course (1º-5º) including the teaching quarter they correspond to and their ECTS worth
- A downloadable Academic program pdf
- A link to fundamental.html

#### FCE (fundamental.html)
Contains descriptive information of the fundamentals of computer engineering subject. Includes:

- Basic data about the subject (ECTS, language, teching quarter, module, area...)
- Introduction to FCE
- Goals
- Course syllabus (contents)
- Education activities
- Skills
- Learning results
- A downloadable teching guide pdf

#### Contact (contact.html)
Contains methods to contact the developer via:

- e-mail
- Instagram (link)
- Facebook (link)

The e-mail contact form does not work due to practical work specifications not specifying it to work.

### Technical Architecture

#### Structure
The website is organized in the following structure from the root (FCEWebsite.github.io) directory:

- README.md
- LICENSE
- /docs
- - /docs/css
- - - /docs/css/main.css (main and only style sheet used fot this project)
- - /docs/images (contains all the images used in the website)
- - /docs/public (contains every other html doc apart from index.html)
- - - /docs/public/about.html
- - - /docs/public/contact.html
- - - /docs/public/degree.html
- - - /docs/public/fundamental.html
- - - /docs/public/net.html
- - - /docs/public/topic.html
- - docs/index.html

Downloadable files (Academic program.pdf, Curriculum.vitae.pdf, IoT.pptx and Teaching guide.pdf are all inside the /docs directory).

#### CSS style
Every html document (web page) uses the same CSS file (main.css), which is referenced externally in every web page.

#### References
Images, links, files or the main.css file are referenced in html documents using relative paths, which is a more common and comfortable way of referencing other files working from the current directory.

#### Imports
The following external imports were made to enhance the project:

- Bootstrap's CSS and JS carousel (in topic.html)
- Google's Montserrat font family (in every document)

---
## Problems Faced
Bellow you will find a discussion of the challenges and problems which were encountered during the development process and how the were managed/solved.

### Issue 1: Relative path changes
> Explain the issue and the resolution.

### Issue 2: Name references incompatiblw on github upload
> Explain the issue and the resolution.

### Issue 3: Columns

### Issue 4: Hover layout distorsion

## Conclusions
> Summarize your learning outcomes from this project. Discuss what was successful and what could be improved.

---
**Note:** This document is part of the practical work II by Marcos García Balboa, developed for the Fundamentals of Computer Engineering course.

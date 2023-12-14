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
During the developement of the website and after the upload of the projecto to the repository there were some major issues regarding paths ansd references (including name reference problems (capital letter incompatibilities) and relative path problems when a file was changed from one directory to another). These issued, however, were easy to get used to and after some time they almost disappeared.

### Issue 2: Name references incompatiblw on github upload
When uploading to github, all of the links stopped working due to capital letter incompatibilities. Including Index.html (which had to be changed to index.html for the browser to interpret ir as the index page). All of the names had to be changed along with the references, which took some time but after it the issue was completely gone.

### Issue 3: Columns
There were several issues regarding aligning obects horizontally, including them going off-screen- some columns being inexplicably bigger than others, divs taking too much space. Many different layout composition models were tried and after some time, the flexbox method turned out to be the most suitable one, as it is direction-agnostic and dynamic accross different screen sizes.

### Issue 4: Hover layout distorsion
When implementing hover animations through hover events and transitions in CSS, hovered items would become bigger and distort the arrangement of other elements of the pages. This is the issue that took the most time resolving, as the aim was a balance of the slightest distorsion possible but still wanting the webpage to feel lively and interactive.

The solution turned out to be compensating the increase in the object size (font and border increase) wirh padding/mergin decreases. However, the transition still made other items displace because, while the border  width change was 1px (1px-2px), the padding diference was 10px (20px-10px) so, even though that when the transition ended objects were arragned the same than when it started, during the transition there was a slight displacement due to frame differences (because, while padding can transition more softly due to ir having more steps in the transitions, border width could only transition 1 time (from 1px- to 2px)). However, the movement was so slight that the advantages were far greater than the disadvantages and the feature was kept.

## Conclusions
> Summarize your learning outcomes from this project. Discuss what was successful and what could be improved.

---
**Note:** This document is part of the practical work II by Marcos García Balboa, developed for the Fundamentals of Computer Engineering course.

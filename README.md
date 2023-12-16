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
Below you will find a discussion of the challenges and problems encountered during the development process and how they were managed or solved.

### Issue 1: Relative path changes
During the development of the website, and after uploading the project to the repository, there were significant issues regarding paths and references. This included name reference problems (such as capital letter incompatibilities) and relative path issues when a file was moved from one directory to another. However, these issues were eventually easy to adapt to, and they almost disappeared over time.

### Issue 2: Name references incompatible on github upload
Upon uploading to GitHub, all of the links stopped working due to capital letter incompatibilities. For instance, 'Index.html' had to be changed to 'index.html' for the browser to recognize it as the index page. All names and references required updating, which was time-consuming, but this resolved the issue completely.

### Issue 3: Columns
Several issues arose regarding the horizontal alignment of objects, including some going off-screen, columns being inexplicably larger than others, and divs occupying too much space. Various layout composition models were tested, and ultimately, the flexbox method proved to be the most suitable. It is direction-agnostic and adapts dynamically across different screen sizes.

### Issue 4: Hover layout distorsion
Implementing hover animations with hover events and transitions in CSS caused hovered items to enlarge and distort the arrangement of other page elements. This was the most time-consuming issue to resolve. The goal was to minimize distortion while maintaining a lively and interactive webpage feel.

The solution involved compensating for the increase in object size (font and border increase) with decreases in padding/margin. However, the transition still caused other items to shift slightly. This was because, while the border width change was minor (1px to 2px), the padding difference was larger (20px to 10px). So, during the transition, there was a slight displacement due to frame differences. The padding transitioned more smoothly because it had more steps, whereas the border width could only change once. Nonetheless, the movement was subtle, and the benefits outweighed the disadvantages, so the feature was retained.

## Conclusions
Programming in HTML and CSS is a great challenge for first-course students who are new to programming or understanding of distributed source code repositories. 

Personally I consider this project as a great opportunity to learn and understand how webp ages/websites work and how source code files are tipically managed. I have enjoyed the development of this project greatly and am really satisfied with my ability to overome issues and with the final results.

---
**Note:** This document is part of the practical work II by Marcos García Balboa, developed for the Fundamentals of Computer Engineering course.

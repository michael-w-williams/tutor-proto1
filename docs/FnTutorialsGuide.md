# Fn Tutorials Guide
This is a guide to creating a tutorial for the FN project. 

## Before You Begin
### Background
The goal of this guide is describe some of the techniques and conventions we use to create Fn tutorials. We want to achieve some consistency in our tutorials but at the same time keeping things simple.

**Note:** As a bonus this guide it written using our tutorial template (provided at the end of this guide) as an example of its use.

### Prerequisites
* An editor for creating Markdown.

### Initial Setup
Follow these steps.

1. Create a directory for your tutorial in the repo.
1. In the directory create an images directory.
1. Copy the ![User Input Icon](https://github.com/fnproject/tutorials/raw/master/Introduction/images/userinput.png) [userinput.png](https://github.com/fnproject/tutorials/raw/master/Introduction/images/userinput.png) into that directory.
1. Create a README.md file using the tutorial template included at the end of this document.
1. Customize the titles, sections, and section titles to meet your needs.

## Formatting
There are a few markdown formatting styles and techniques we use in our tutorials. The Jekyll theme relies on these to build HTML pages.

### Titles and Sections
The tutorial title should be an h1 (#). Each section should start with and h2 (##). Try to use action verbs telling the learner what to do in section titles. For example, "Start Fn Server".

### User Actions and Graphic
Each time you want the user to do something precede that step with an icon followed by the command with the following format. For example:

![User Input Icon](https://github.com/fnproject/tutorials/raw/master/Introduction/images/userinput.png)

>```sh
>export ENV_VAR=VALUE
>```

This format combines a blockquote with a code block to provide a unique way to identify a command.

If you don't want syntax highlighting for your command or are showing an Fn command that won't be syntax highlighted, you can use simple syntax. For example:

![User Input Icon](https://github.com/fnproject/tutorials/raw/master/Introduction/images/userinput.png)

>`fn start`

It save some typing and still looks decent.

**Note:** Jekyll uses the [Rouge Syntax Highlighter](https://github.com/jneen/rouge) for code blocks. See that documentation for languages supported. 


## Tutorial Template
Here is a template for creating a tutorial. Note the only required elements are a "Title" and at least one "Step Section". The "Before you Begin" and "Learn More" sections are recommended but not required.

```markdown
# Tutorial Title (Required)
Each tutorial must have a title. 

## Before you Begin (Recommended)
Provides you the why about this tutorial.  Also covers any  required setup to do the tutorial.

### Background (Optional)
Provides a information about what the tutorial covers and what you will learn. Covers the why of the tutorial.

### Prerequisites(Optional)
Spells out any activities or tools that are required before starting the tutorial.

## Section (At least 1 Required)
You must have at least 1 step/section for a tutorial. You do not need to number the steps.

## Additional Section (Option)
Create as many sections as you need. Use or don't use Section steps (### and ####) as you need.

### Section Step (Optional)
One step in this section.

### Section Step (Optional)
One step in this section.

#### Section Sub-Step
Sub-step if needed.

#### Section Sub-Step
Sub-step if needed.

## Learn More (Recommended)
Links to resources where learners could go to learn more about this topic.

* Link
* Link
* Link
```

## Learn More
* [Fn Project](https://github.com/fnproject/fn)
* [Fn Project Tutorials](https://github.com/fnproject/tutorials)

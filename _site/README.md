# Standard Operating Procedures
Here is the repository where we can work on developing, updating, and
modifying standard operating procedures for the office.  The information
below should help you to add to the document.  Currently the majority of
the document is just an outline.

# What you will need
You can edit the markdown files in any editor you choose, but you'll
need to make sure that you have `Ruby` installed on your machine.  Once
installed move to this directory and execute the following:

```
# Set the project root variable with the name of the directory that 
# contains this repository on your machine
PROJECT_ROOT=/Users/billy/Desktop/Programs/other/

# Assuming you are using a bash shell this will move you into the directory
cd "${PROJECT_HOME}/fcps-standards"

# Now install the Ruby gems that are needed to generate the HTML and 
# serve up the content locally so you can see how it looks and runs
bundle install

# Now you should be able to serve up the content locally:
bundle exec jekyll serve
```

This should return output in the console that looks something like:

```
billy-2:fcps-standards billy$ bundle exec jekyll serve
Configuration file: /Users/billy/Desktop/Programs/other/fcps-standards/_config.yml
       Deprecation: The 'gems' configuration option has been renamed to 'plugins'. Please update your config file accordingly.
            Source: /Users/billy/Desktop/Programs/other/fcps-standards
       Destination: /Users/billy/Desktop/Programs/other/fcps-standards/_site
 Incremental build: disabled. Enable with --incremental
      Generating... 
                    done in 2.158 seconds.
 Auto-regeneration: enabled for '/Users/billy/Desktop/Programs/other/fcps-standards'
    Server address: http://127.0.0.1:4000/fcps-standards/
  Server running... press ctrl-c to stop.
```

If it does and you go to `http://127.0.0.1:4000/fcps-standards/` you should
be able to view the content from your machine.

# How to move forward
1. Fork the repository on GitHub
2. Clone the repository on your machine
3. Create a new branch named for what you are adding and checkout that branch (see example below)
4. Make modifications to the content
5. Run `bundle exec jekyll build` if you already know what it looks like or `bundle exec jekyll serve` if you need to build and view things
6. Commit the changes in the same branch that you were working on
7. Submit a pull request

# New Sections
The information below will explain how to add new sections to the
documentation.  You should be able to copy and paste the examples as
needed to create new content.

## Section - Header File
Each section should have its own root level file with directives to
include all of the related files.  The `layout` shall be `page` and the
`permalink` shall be constructed using snakeCase and be the same value
as the name of the file for the new section.  The `title` field in the
front matter should be as short as possible while still being
sufficiently descriptive.

```
---
layout: page
title: Code
permalink: /codingStandards/
---

{% include codingStandardsTOC.md %}

# <a name="codingStandards"></a> Coding Standards

[Back to the Top](codingStandards.md#top)  [Back to Table of Contents](codingStandards.md#codingStandardsTOC)

{% include purpose.md %}

{% include fileSystem.md %}

{% include naming.md %}

{% include documentation.md %}

{% include whenToDev.md %}

{% include vcs.md %}

{% include codeStyle.md %}

{% include codeReview.md %}

{% include qaqc.md %}

{% include testing.md %}

```

The order in which the files are referenced should match the order they
appear in the table of contents file associated with this section.

## Section - Table of Contents File
Each section needs to have a table of contents.  This will help organize
the work on each section and will also provide a standardized process
for adding to the SOPs moving forward.  The example below is the table
of contents file for the coding standards section.

```
# <a name="codingStandardsTOC"></a> Coding Standards

## Table of Contents

* [Coding Standards](_includes/codingStandardsTOC.md#codingStandards)
	1. [Introduction](_includes/codingStandardsTOC.md#purpose)
	2. [File System Management](_includes/codingStandardsTOC.md#fileSystem)
	    * [File Naming Conventions](_includes/codingStandardsTOC.md#fileNames)
	    * [Directory Tree Structure](_includes/codingStandardsTOC.md#directoryTree)
	    * [Versioning Files](_includes/codingStandardsTOC.md#fileVersions)
	3. [Naming Conventions](_includes/codingStandardsTOC.md#naming)
	    * [Naming Style](_includes/codingStandardsTOC.md#nameStyle)
	    * [Demographic Data](_includes/codingStandardsTOC.md#demographics)
	    * [Assessment Data](_includes/codingStandardsTOC.md#assessment)
	4. [Documenting Code](_includes/codingStandardsTOC.md#documentation)
	    * [Literate Programming](_includes/codingStandardsTOC.md#literateProgramming)
	    * [File Headers](_includes/codingStandardsTOC.md#fileHeader)
	    * [Block Comments](_includes/codingStandardsTOC.md#blockComments)
	    * [In-line Comments](_includes/codingStandardsTOC.md#inlineComments)
	5. [Development Guidance](_includes/codingStandardsTOC.md#whenToDev)
	    * [Reusability](_includes/codingStandardsTOC.md#codeReuse)
	    * [Replicability](_includes/codingStandardsTOC.md#replicable)
	    * [Reliability](_includes/codingStandardsTOC.md#reliability)
	    * [Responsibility](_includes/codingStandardsTOC.md#responsibility)
	6. [Version Control](_includes/codingStandardsTOC.md#vcs)
	    * [Git: Live it, Learn it, Love it](_includes/codingStandardsTOC.md#git)
	    * [Repository Initialization](_includes/codingStandardsTOC.md#gitInit)
	    * [Staging Code for Commit](_includes/codingStandardsTOC.md#gitAdd)
	    * [Committing Code to Repository](_includes/codingStandardsTOC.md#gitCommit)
	    * [Pushing Changes to Remote Repository](_includes/codingStandardsTOC.md#gitPush)
	    * [Getting Changes from Remote Repository](_includes/codingStandardsTOC.md#gitFetch)
	    * [Combining Changes from Other Repositories/Branches](_includes/codingStandardsTOC.md#gitMerge)
	    * [Pull Requests](_includes/codingStandardsTOC.md#pullRequests)
	    * [Code Contributions](_includes/codingStandardsTOC.md#contributingCode)
	7. [Style Guides](_includes/codingStandardsTOC.md#codeStyle)
	    * [Stata](_includes/codingStandardsTOC.md#Stata)
	    * [R](_includes/codingStandardsTOC.md#R)
	    * [Java](_includes/codingStandardsTOC.md#Java)
	    * [SQL](_includes/codingStandardsTOC.md#SQL)
	    * [Bash](_includes/codingStandardsTOC.md#bash)
	    * [C#](_includes/codingStandardsTOC.md#CSharp)
	    * [Visual Basic](_includes/codingStandardsTOC.md#vb)
	    * [Julia](_includes/codingStandardsTOC.md#Julia)
	    * [Python](_includes/codingStandardsTOC.md#Python)
	    * [Batch](_includes/codingStandardsTOC.md#batch)
	8. [Code Reviews](_includes/codingStandardsTOC.md#codeReview)
	    * [Reviewing Code](_includes/codingStandardsTOC.md#reviewingCode)
	    * [Checking Style](_includes/codingStandardsTOC.md#checkingStyle)
	    * [QA/QC](_includes/codingStandardsTOC.md#qaqc)
	9. [Collecting Business Rules](_includes/codingStandardsTOC.md#businessRules)
	    * [User Stories](_includes/codingStandardsTOC.md#userStories)
	    * [Epics](_includes/codingStandardsTOC.md#epics)
	    * [Projects](_includes/codingStandardsTOC.md#projects)
	10. [Testing](_includes/codingStandardsTOC.md#testing)
	    * [Unit Testing](_includes/codingStandardsTOC.md#unit)
	    * [Regression Tests](_includes/codingStandardsTOC.md#regression)    
	    * [User Acceptance Testing](_includes/codingStandardsTOC.md#uat)
```

Notice that the links all resolve to anchor tags defined as `subdirectory/fileName.md#name`.  
This allows the links that are generated by [jekyll](https://jekyllrb.com/) to resolve the
markdown correctly to point at the appropriate HTML identifiers.

## Section - Content Files
When templating, the first set of links that should appear in a contents
file should be:

```
[Back to the Top](_includes/whenToDev.md#top)  [Back to Table of Contents](_includes/whenToDev.md#codingStandardsTOC)
```

This allows the user to navigate back to the top of this section, or
back to the table of contents for that SOP.  As subsequent subsections
are added to the file, the list of links should also provide an option
that allows a user to return to the top of the current sub-section, the
top of the major section, or to the table of contents (e.g., top of
document).

```
## <a name="whenToDev"></a> 5. Development Guidance

[Back to the Top](#whenToDev)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="codeReuse"></a> Reusability

[Back to the Top](#codeReuse) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

### <a name="replicable"></a> Replicability

[Back to the Top](#replicable) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

### <a name="reliability"></a> Reliability

[Back to the Top](#reliability) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

### <a name="responsibility"></a> Responsibility

[Back to the Top](#responsibility) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)
```
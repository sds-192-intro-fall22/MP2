# Mini-Project 2

# Overview

> Please note that many aspects of this project are informed by similar projects designed for Professor Albert Kim's and Professor Ben Baumer's SDS 192: Introduction to Data Science courses at Smith College. 

Every year the U.S. Federal Election Commission publishes data that details how candidates and committees raise and spend money in federal elections. In this mini-project, you will perform some data wrangling in order to extrapolate insights from the FEC's campaign contributions dataset in the 2015-2016 election cycle. You will then write up your findings in a short blog post (400-500 words). You will be expected to engage the data wrangling verbs, perform at least one join, and showcase your ability to collaborate effectively in GitHub. In your blog post, you will detail how the data in this dataset was produced, along with what we learn through data wrangling. 

To access the data for this project, you will engage the `fec16` package developed by fellow Smithies: Prof Ben Baumer, Rana Gahwagy, Irene Ryan, and Marium A. Tapal! 

# Learning Goals

* Apply the verbs of data wrangling to produce insights from data
* Join data across multiple tables
* Effectively collaborate with team members in GitHub
* Communicate data findings in writing
* Evaluate the ethical dimensions of data resources

# Detailed Instructions

## Establish a GitHub Workflow

In this lab, I will expect you to develop a GitHub workflow for the project submission. This means that all group members should create issues associated with tasks they are assigned to in GitHub, work in separate branches of the repo to make those changes, and issue Pull Requests to merge their changes into the project. You should also establish a review process to review each other's code before merging. 

1. After reading all of the requirements of this project, I recommend that you delegate tasks amongst group members, start recording those as Issues in the GitHub repo, and assign Issues to group members. 

2. Create separate branches of the repo for each team member.

3. Decide who will be group member 1, 2, 3, and so on.

## Set up your environment

4. In RStudio, `File` > `New Project` > `Version Control` > `Git` and then copy the URL to this repo. **Switch to your branch.** 

5. Open `fec_analysis.qmd` and add your name to the header at the appropriate location (lines 5, 7, and 9). Keep in mind that if you enter your name in the same line number as one of your teammates, you will be dealing with a merge conflict later. This is why it was important to assign numbers in Step 3. At this point I would recommend that you save the file, stage and commit your changes, push the changes to GitHub, have all team members issue their first pull request, merge all of the changes, delete the personal branches, and then recreate the branches for the next round of changes. This will help you practice the workflow and work out any kinks early on. After you've followed these steps, be sure to pull the changes back into RStudio before moving on with the project. 

4. Install the `fec16` package:

`install.packages("remotes")`
`remotes::install_github("baumer-lab/fec16")`

## Get to know the FEC data

5. Read about the history and mission of the FEC [here](https://www.fec.gov/about/mission-and-history/).

6. You should review this [README](https://github.com/baumer-lab/fec16) as a reference for the data included in these files and as inspiration for your project. Note however, that you may not use the examples in these vignettes in your submission.  

## Wrangle the Data

7. As a group, devise a question about the 2015-2016 campaign contributions, spending, and/or results that you would like to answer with your data. Your question should be concise and should be a question that can be answered with the data available to you via descriptive data analysis. Avoid questions that require predictive analysis or analysis of variables not represented in this dataset.

8. Write one code chunk per team member that leverages some combination of the 6 data wrangling verbs to produce a table or a plot that offers insight into campaign contributions, spending, and/or results in the 2015-2016 election cycle. You must both subset and aggregate the data in some way, and use at least one join in the analysis. All plots must be labeled with all five components of data context. You may help each other write your code chunks, but every team members should ultimately push their own chunk to GitHub.

> Note that I recommend that you try your best to work within the lines allotted to you, without adding new lines to your code chunk. This means using the down arrow instead of the return key to move to a new line. This will help avoid merge conflicts later on. ...even though I fully trust that you'll become whizzes at fixing those when they arise! :)

9. All code chunks must be reviewed on GitHub.com by at least one other team member following a pull request and before merging, and all team members must review at least one chunk. Reviewers may request changes to the code, edits to the comments, suggestions for better labeling/aeshetics, and/or simply commend their peers' work@ The course grader and I will be checking for this when evaluating your submission.

## Write blog post

> Note that you do not need to use the long and elegant GitHub workflow for composing the blog post, as I understand that many students would perfer to write this up in Google Docs and the copy it over to RStudio. The long and elegant workflow is only required for the coding sections of the project. 

10. In 400-500 words, you should write a blog post reporting on your visualization:
  * Paragraph 1: Introduce the dataset and the question you posed when approaching the analysis. 
  * Paragraph 2: Report on findings from your analysis.
  * Paragraph 3: Summarize the key takeaway from your analysis and describe at least one ethical concern we should consider when joining data across data frames.
    
## Record standards and submit assignment

11. Open `standards.qmd`, and under each heading, indicate how the work you completed for this project demonstrated fluency in that standard. You may wish to reference the Evaluation section below for help with writing this up. 
12. Open `contributions.qmd` and briefly describe each team member's contributions to the project. 
13. When you are done, you should save all .qmd files, render the documents, commit changes, and then push changes back to GitHub. That's it for submission. You don't need to submit anything on Moodle. 

# Evaluation 

You will be evaluated on the extent to which your mini-project demonstrates fluency in the following course learning dimensions:

* Transforming Data
  * 1 point - Demonstrates an ability to subset data
  * 1 point - Demonstrates an ability to aggregate data
  * 1 point - Demonstrates an ability to interpret the results of data wrangling
* Joining Data
  * 1 point - Demonstrates an ability to join to data frames
  * 1 point - Demonstrates an ability to select the most appropriate type of join
  * 1 point - Demonstrates an ability to reflect upon ethical concerns of joining information across data frames
* GitHub
  * 1 point - Demonstrates an ability to delegate tasks effectively via Issues
  * 1 point - Demonstrates an ability to collaborate across multiple GitHub branches
  * 1 point - Demonstrates an ability to review collaborators' code
  


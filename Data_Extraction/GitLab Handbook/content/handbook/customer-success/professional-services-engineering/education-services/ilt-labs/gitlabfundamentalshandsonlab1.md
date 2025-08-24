---
title: "GitLab Fundamentals - Hands-On Lab: Organizing your work in GitLab"
description: "This Hands-On Guide walks you through the basics of organizing and structuring your work in GitLab."
---

> Estimated time to complete: 30 minutes

## Objectives

In this lab, we will explore how we can organize work in GitLab, using groups, sub-groups, and projects.

## Task A. Viewing a group structure

To start, in the left sidebar, select **Groups**.

1. In the **Groups** section, select the dropdown arrow on the left of **Training Users**. 

1. Below **Training users**, you should now see a group with a name like **Session <string of characters and numbers**.

1. Click the dropdown arrow next to the **Session** group. You should now see a group named **My Test Group - <string of characters and numbers>**. Click this group to access it.

This navigation shows an example of groups and subgroups. In the ILT GitLab instance, the **Training Users** group is a top-level group. This means that it is not part of any other groups in the instance. The **Training Users** group contains a set of subgroups, which represent classes running in the instance. Each of these subgroups is given a name like **Session <string of characters and numbers>**. Inside of these groups is a set of subgroups, one group for each student in the class. The **My Test Group** subgroup is your own group, which you can organize and modify in any way you like.

## Task B. Creating a Group Structure

To start, make sure you are in the **My Test Group** subgroup. For this task, imagine you are working at a company with two departments: Development, and QA. These departments have the following projects:

- Development: A mobile and desktop version of an application named `Cool App`. Of note, `Cool App` contains many microservices spread over many repositories for both versions.
- QA: Two testing frameworks, one for the mobile version of `Cool App` and one for the desktop version. Both frameworks are monolithic, stored in a single project.

Take some time here to consider a structure for these two teams. After considering options, take a look at the steps below for a possible solution.

1. Since we have two teams, let's create a group for each team. Select **New subgroup**. 

1. In the **Subgroup name**, enter `Development`. Leave all other options as default and select **Create subgroup**.

1. At the top of the page, you will see a set of breadcrumbs which shows your location in the application. Click **My Test Group** to return to your main group.

1. From here, you will now see your `Development` group. Select **New subgroup** to create your group for QA.

1. In the **Subgroup name**, enter `QA`. Leave all other options as default and select **Create subgroup**.

1. Select **My Test Group** from the breadcrumbs again to return to your main group. You will now see two groups: `Development` and `QA`. 

Next, we can structure subgroups for both team's projects. Since the development applications have many projects, it makes sense to create a subgroup for each project type.

1. Select the `Development` group.

1. Select **New subgroup**.

1. In **Subgroup name**, enter the name `Cool App Desktop`. Select **Create subgroup**.

1. In the breadcrumbs, select **Development** to return to the development group.

1. Select **New subgroup**.

1. In **Subgroup name**, enter the name `Cool App Mobile`. Select **Create subgroup**.

1. In the breadcrumbs, select **Development** to return to the development group.

Now in the `Development` group, you will see a `Cool App Desktop` and `Cool App Mobile` subgroups, ready to contain any projects related to both applications.

For the QA team, they have a single project. There are two main options for structuring this team. We can create a group for `Cool App Testing` that will contain the project, or we can just create the project in the subgroup.

## Task C. Creating a repository

Let's create a new repository for the QA team. Select the `QA` group in your **My Test Group**. From here:

1. Select **New project**.

1. Select **Create blank project**.

1. In the **Project name**, enter `Cool App QA`. 

1. Ensure that **Initialize repository with a README** is checked on. This will create a README file in the project as a starting point.

1. Select **Create project**.

After creating the project, you will be navigated to the repository of the project. You will see a single file titled `README.md`, which contains a basic README template. To get started working with this project, let's create an issue.

## Task D. Creating issues in a project

Let's learn the basics of creating issues in GitLab. 

1. Navigate to your **Cool App QA** project. 

1. In the left sidebar, select **Plan > Issues**. 

1. Select **New issue**.

1. In the title, enter `First issue`.

1. Enter any description you like.

1. Select **Create issue**.

By following this process, you created an issue related to your **Cool App QA** project. Let's discuss some of the details related to your issue. In the center, you will see your issue description, as well as activity for the issue and an area to add comments and discussions. Every issue can have child items, which are smaller tasks related to the issue. Issues can also be linked to other issues to show relationships between issues. 

In the right sidebar, you will see metadata related to your issue. The **Assignee** is the set of people currently working on the issue. If the issue is associated with an epic, milestone, or iteration, these details will display here. Labels can be added to an issue to help organize issues into similar categories or types. Weight defines the amount of work associated with an issue. A due date can be set on an issue for when it should be completed by. Time tracking lets you track time taken to complete an issue. Health status lets you set a status for how the issue is progressing.

Often, we use issues to represent smaller pieces of work that may be completed in a single iteration or sprint. For larger sets of work, we use the concept of an epic, which will be discussed in a later lab.

## Lab Guide Complete

You have completed this lab exercise. You can view the other [lab guides for this course](/handbook/customer-success/professional-services-engineering/education-services/ilt-labs/gitlabfundamentalshandson).

## Suggestions?

If you'd like to suggest changes to the lab, please submit them via merge request.

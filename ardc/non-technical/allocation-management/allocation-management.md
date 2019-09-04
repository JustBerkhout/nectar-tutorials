---
id: allocation-managment
summary: Understand, manage and maintain an allocation in the Nectar Research Cloud
categories: non-technical
tags:  expiry bot amend extend user management project manager delegation allocation
difficulty: 2
status: draft
feedback_url: https://github.com/JustBerkhout/tutorials.ubuntu.com/issues
published: 2019-09-02
author: Just Berkhout <just.berkhout@utas.edu.au>

---

# Allocation Management

## Overview

*Allocations, Quota, Resources, Accounts, Projects...* These are some of the words that we use here at Nectar to help you and other Nectar users organise access to the Nectar Research Cloud. Making the most of the Nectar Research Cloud requires that you familiarise yourself with this language and with the associated processes. 

Nectar Cloud resources are granted to you in periods of up to a year. An automated expiry process will recover unused and unclaimed resources and the recovered resources can then be granted out to researchers just like yourself. 

negative
: **Warning**
Familiarise yourself with the expiry process, to prevent surprise deletions of your hard work and data. 

negative
: **Antarctica and Amazon (the rainforest)**
The Expiry Bot diligently executes the expiry process. It does not know of your field trips to Antarctica or the Amazon rainforest, or any other places where wifi-access or your attention to emails may be limited. Make sure you have arranged extensions for your projects if you happen to be away for extended periods or delegate your project manager role to another user. 

### What you'll learn

- Understanding *accounts*, *allocations*, *projects*, *resources* and *quota*
- Requesting and Amending allocations
- *Allocation expiry*
- Delegating the *Project Manager* role to another user

### What you'll need

- A Nectar Research Cloud account, or access to the AAF to get one. 



## A diagram

Duration: 2:00

![Overview diagram](images/requests-projects.svg)

### 

## Accounts and Personal Trial (pt) projects

Duration: 5:00

The first time you log on to the dashboard, Nectar creates two things your *Account* and a *Personal Trial (pt)* project. Your account is tied to your email address, while your personal trial is a project named pt-*xyz* (where *xyz* is a number). The two are closely related, but they are not the same thing.

### Your Nectar Account

You log on to [Nectar dashboard](https://dashboard.rc.nectar.org.au/) using [AAF](https://aaf.edu.au/) (in Australia) or [Tuakiri](https://www.reannz.co.nz/products-and-services/tuakiri/) (in New Zealand). AAF and Tuakiri provide both authorisation and authentication, using your identity (i.e. username) at your home institution.

You account is created upon your first logon. You account is associated with your email address and will contain some account-related information, such as your public-private key pairs (when you register them), your Nectar OpenStack password or any Application Credentials you might create. 

positive
: Your Nectar OpenStack password is not the same thing as your AAF/Tuakiri password. Read more about the Nectar OpenStack password in our [knowledge base article](https://support.ehelp.edu.au/support/solutions/articles/6000145832-the-nectar-openstack-password). Note also that [Nectar OpenStack Application Credentials](https://support.ehelp.edu.au/support/solutions/articles/6000212274-application-credentials) are a more sophisticated solution than the Nectar OpenStack password.

### Your pt-project

Upon your first logon Nectar creates a trial project for you, known as your *pt*-project (or *personal trial*). In this project you are allocated a very limited quota of 2vCPU of resources for a maximum of 6 vCPU-month of running time. 

Your pt-project is like a full-fledged project in many ways. It is the home of instances, it has quota of some resources allocated (e.g. vCPU, RAM), it houses your project-related things, such as Security Groups

In other ways your pt-project is different from full-fledged projects. It has *limited resources* (2 vCPU for up to 6 vCPU-months). You can't share you pt-project with others; the is no user management to grant access to other Nectar users. You get your pt *no questions asked*; there is no application or allocation process. Your *pt-project* is useful for trialing or indeed completing Nectar tutorials.

After you have used all the compute time allocated to you in your pt-project it will expire. If you have built up anything valuable in your *pt-project* you can request that we *Convert you trial project* when you submit a request for a project allocation. Note that the Expiry Bot will start removing instances from your pt-project shortly after pt-project expiration. To retain them by using a trial project conversion, you need to request a project timely. More detail in the section Project Trial in our article on [Expiry and Renewal](https://support.ehelp.edu.au/support/solutions/articles/6000171494-project-allocation-expiry-and-renewal) 

## Allocation Process and Projects

Duration: 5:00

To get a full-fledged project allocated to you you need to apply for an allocation using the`Allocation | New Request` form available from your Nectar dashboard. Once approved you will be informed by email and you will be the *project manager* of your new project. 

![Allocation request](images/allocation-request.png)

To be eligible for a Nectar national allocation you have to submit details of your nationally relevant grant or funding program. If you don't have such a grant, then you can still be allocated cloud resources by the participating nodes under node discretion, by specifying a *Allocation home location* in your request. 

In your request you need to specify the cloud resources that you intend to use. If you're not perfectly sure just yet, then that's all right. You will be able to request amendments to your project. We'll describe that below. 

positive
:  More info can be found in the section [Allocations](https://support.ehelp.edu.au/support/solutions/folders/6000230417) in our knowledge base, including our current [Research Cloud National Allocation Scheme (RC-NAS) Policy](https://support.ehelp.edu.au/support/solutions/articles/6000191233-research-cloud-national-allocation-scheme-rc-nas-policy-)

### Allocation requester and project manager

The user that requests an allocation/project will automatically become both a Member and the Project Manager of that project when it is approved. 

Project managers have access to a few functions that ordinary project members don't have:

- User management
- Project listed in *My Requests*, *Amend/Extend* ability
- Allocation and Expiry process communications

positive
: Occasionally you might come across the term *tenancy* or *tenant-manager*. These art depr'cated words meaning *project* and *project manager* respectively. 

## Amending and Extending

Duration: 2:00

To change the resources allocated to your project or to extend the duration of your project you or another project manager can submit an Amend/Extend request. 

To submit an Amend/Extend request follow these steps.

1. On your Nectar Dashboard, Navigate to the `Allocations | My Requests` page
2. Click the `Amend/Extend allocation` button.

You will go to the Allocation Request form, with some of your project's details already filled in. From time to time the Allocation Request form changes, so please read or reread the form when filling in the requested details. 

![](images/amend-extend-allocation.png)

## Project Expiry

Duration: 2:00

Project allocations on the Nectar Research Cloud are created for a fixed term to help ensure fair access to resources for all users of the cloud. When a project allocation nears the end, project managers and members are notified via email. 

The expiry process is an automated process that follows the rules that are set out in our article on [Expiry and Renewal](https://support.ehelp.edu.au/support/solutions/articles/6000171494-project-allocation-expiry-and-renewal). 

negative
: **Warning** 
Familiarize yourself with the expiry rules: the *Timeline*, *Action by Nectar* and the *Options for Users*. The last step of expiry -after a generous grace period- is that Nectar deletes the project's resources. Yes. *Deletes.*  [Expiry and Renewal](https://support.ehelp.edu.au/support/solutions/articles/6000171494-project-allocation-expiry-and-renewal) article here. 

## Share or delegate the *project-manager* role

Duration: 4:00

If you need to ensure that your project doesn't expire, you can also share the *project-manager* role with other users in your project. All users in the project that have the *project-manager* role will be notified of the stages of expiry by the Expiry Bot, and they have access to the `Amend/Extend allocation` button for the project via the My Requests page. 

To sha./re	re/delegate you need to take two steps:

1. If the user you would like to share the *project-manager* role with isn't in your project, then you need to add them as a Member to your project using the User Management feature. 
2. To assign the *project-manager* role to a Member of your project you need to contact Nectar support

### Add Members

To add members to your project, follow these steps:

1. On you nectar dashboard ensure you have the correct project selected in the Project selector 
2. Navigate to the `Identity | Project Members` page 
3. Click the `Add` button to open the `Add User to Project` dialog
4. Enter the user's Username (i.e. the email address) and click the `Add User to Project` button

Note the User's usename must be an existing account in Nectar. If you are unsure, ask the user to log in to Nectar and use the email address they have in the top right hand corner of the dashboard.

![Adding a Project Member](images/add-project-member.png)

### Contact Nectar support

To assign the *project-manager* role to an existing user in your project, you or another project-manager needs to contact Nectar Support. You can use the `Support Ticket` link from your dashboard, send an email to support@ehelp.edu.au or log a ticket on [support.ehelp.edu.au]( https://support.ehelp.edu.au/support/tickets/new), requesting that the project member be assigned the project manager role, and whether you yourself need to retain project-manager status.

Note that Nectar will only accept requests for assigning the project-manager *from existing project-managers* or from the Chief Investigator as listed in the project allocation request. 

## Next Steps

Duration: 1:00

In this tutorial you've learnt about Allocation Management. You've learnt what sets *pt-projects* apart from *projects*. You've learnt how to avoid *data-loss-by-expiry* by Amending/Extending your project and you've learnt how to share/delegate your project-manager role with other members of your project. 

All we hope for in return is that you remember us fondly, when you're in [Sweden](https://www.nobelprize.org/ceremonies/the-nobel-prize-award-ceremonies-and-banquets/) next.
---

id: applications
summary: Learn to quickly build and deploy application environments by assembling your favourite apps from our catalog.
categories: Beginner
tags: Cloud Starter, application, dashboard
difficulty: 1
status: draft
feedback_url: https://github.com/JustBerkhout/tutorials.ubuntu.com/issues
published: 2019-08-15
author: Mark Endrei <mark.endrei@uq.edu.au>


---

# Applications

## Overview

Duration: 10:00

### What are Applications

Nectar have packaged some cloud-ready applications into the *Application Catalog* available from your [Nectar dashboard](https://dashboard.rc.nectar.org.au). You can browse the catalog and compose your own application environments running on the Nectar Research Cloud.

In this tutorial you'll step through the *Quick Deploy* process for configuring and deploying and application from the catalog.

positive
: **Cloud Starter**
This tutorial is part of the Nectar Cloud Starter curriculum. You should have a Keypair and you should have terminal software installed on your machine. If you think you need help with any of that, you should complete Cloud Starter tutorials before you start here. 

### What you'll learn

- Deploy an application environment in your Nectar Project

### What you'll need

- Keypair
- [Terminal software](https://support.ehelp.edu.au/support/solutions/articles/6000223964-terminal-software)
- Access to a Nectar Project

## Browsing the Application Catalog

Duration: 3:00

In this tutorial we will browse the Application Catalog and use *Quick Deploy* to configure your own instance of R-Studio running on Nectar. 

1. Log on to on your [Nectar Dashboard](https://dashboard.rc.nectar.org.au) and ensure you're working in the right project (Use the project selector on the top left-hand side)
2. Navigate to the `Applications | Browse | Browse Local` page 
3. If you don't immediately see the application you need, just type it into the search field on the right. For this tutorial, let's find `R-Studio`
4. Once you've found it, click `Quick Deploy`.

![Browse the applications catalog](images/rstudio-browse.png)

## Configure the Application

Duration: 2:00

`Quick Deploy` guides you through the steps to configure your application environment.

### Flavor and Key Pair

Choose your desired **Instance Flavor**, **Key pair** and the **Availability Zone**. Click `Next` to continue.

positive
: With R-Studio you can select an existing volume for application data storage. If you plan to use an existing volume, make sure your volume and application environment are in the same Availability Zone.

![Launch details](images/rstudio-flavor.png)

### Hone name and DNS Zone

You can choose an optional **Host name** and **DNS zone** name for your instance. If you choose a DNS zone at this stage, we will automatically create a DNS entry for you and provision a HTTPS security certificate for your instance.

![Launch Source](images/rstudio-dns.png)

### Existing Volume

Select your volume, if required. Click `Next` to continue.

![dashboard-filters](images/rstudio-volume.png)

### User Details

In this step, you should provide your desired **Username** and **Password** for R-Studio. You will be prompted for these later once the application has been deployed. Click `Next` to continue.

![launch flavor](images/rstudio-user.png)

The last step allows you to provide a name. You can keep the default, *R-Studio*, or supply your own. Click `Next` to continue.

## Deploy the Environment

Duration: 10:00

### Start the Deployment

When you finish configuring the application you will be taken to the Application Environments screen. You'll want to click the `Deploy This Environment` button to kick off the deployment.

![Launch networks](images/rstudio-deploy.png)

The application is now being deployed. This usually takes around 5 to 10 minutes to complete the setup process.

![Launch networks](images/rstudio-deploying.png)

### Environment Deployed

Your application is now deployed and ready. You should see the **Last Operation** message appear with the Internet address of your application instance. You can click this link to get started.

![Launch Security groups](images/rstudio-deployed.png)

## Try Out Your Application

Duration: 5:00

Once you log in with the **Username** and **Password** you provided earlier, you will reach the R-Studio landing page in this example.

You can launch R-Studio from here. We also provide a link to Shiny Server that has also been installed, and a link to access the instance desktop via browser.

![Launch Building](images/rstudio-landing.png)

R-Studio will require you to log in again with the **Username** and **Password** you provided earlier.

![Launch Building](images/rstudio-signin.png)

R-Studio is now available!

![Launch Building](images/rstudio-console.png)

This application also offers access to R-Studio through *Remote Desktop* via *X2Go*. This might be especially useful for workloads that require visualisations that can't be handled from within the browser environment.

If you would like to use the Remote Desktop interface, you should install the *X2Go client*. It is available for Windows, Mac and Linux.

Once installed and running, you should click the `Create Session` button and provide the Host, Login and SSH keypair details. Session type should be XFCE.

![Launch Building](images/rstudio-x2go.png)

Once you have created the session, once you connect, the XFCE graphical environment will appear, and you can launch R-Studio from the menu.

![Launch Building](images/rstudio-desktop.png)

You can also access your R-Studio instance using SSH, with the username and key pair you provided earlier (please see above).

## Next Steps

Duration: 1:00

You have launched an application environment in the Nectar Research cloud. You have used the Quick Deploy process from the Nectar dashboard. You configured and deployed the application then confirmed that it is up and running on the Nectar cloud.

Upon successful deployment your Nectar dashboard shows an active application environment on the `Environments` page.

positive
: **Cloud Starter**
Congratulations. You've deployed an application from the Application Catalog. Now what?

Our next tutorial will show you how to use the Nectar Database feature to deploy relational databases.

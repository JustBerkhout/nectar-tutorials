---
id: nectar-keypairs
summary: Understanding Public-Private Keypairs in the Nectar Research Cloud.
categories: nectar computing
tags: security authentication
difficulty: 1
status: draft
feedback_url: https://github.com/JustBerkhout/tutorials.ubuntu.com/issues
published: 2019-05-07
author: Just Berkhout <just.berkhout@utas.edu.au>

---

# Creating a keypair for use in Nectar

## Overview
Duration: 2:00

In this tutorial you will learn how to create a Public-Private keypair for use with the Nectar Research Cloud. You will learn one or more methods of creating the keypairs and how to import your public key into your Nectar account.

positive
: **Cloud Starter**
This tutorials is part of the Nectar Cloud Starter curriculum. Only the bare essentials of keys are discussed here for Launching a Nectar VM from the Nectar Dashboard.

### What you'll learn

- How to create a Public-Private keypair for use with your Nectar Virtual Machine/s
- How to import your Public key into your Nectar account

### What you'll need

- A terminal that has the `ssh-keygen` app installed, or
- PuttyGen (if you're on Windows and intend to use Putty)
- Access to the Nectar Research Cloud

## About keys and Nectar
Duration: 4:00

A Public-Private keypair is used in the Nectar in stead of a password, to log on to any Virtual Machine (VM) that Nectar launches for you. You will learn more about Launching in another tutorial and you will learn about `ssh`-connecting to your VM in a third. 

Before you get to that, you need to have a keypair and register your Public key in your Nectar account. 

A Public-Private keypair is a pair of files, you r Private key and your Public key. They uniquely belong to each other. Your Private key file is yours, and yours alone. You should securely store it on a location on your computer that is only accessible to you.  Your Public key can be used to authenticate you in a remote computer account. 

When you launch an instance, Nectar places the Public key from your Nectar account into your VM for you, attached to an admin user account.  

This way you can use `ssh` to connect to your VM using its IP address, the user account, and the private key that is securely stored on your computer.

Let's get a keypair and register it in Nectar. 

## Nectar convenience method
Duration: 2:00

Nectar can generate a keypair for you. It's easy and it means that your Public key is automatically registered in your Nectar account. You will have to ensure that your downloaded Private key file is in an appropriate and secure location on your computer.

To get your Nectar-generated key you follow these steps

- Logon to the [Nectar Dashboard]([https://dashboard.rc.nectar.org.au](https://dashboard.rc.nectar.org.au/)) and navigate to Key Pairs page
- Click the "**+** Create Key Pair" button

![key-pairs-page](images/key-pairs-page.png)

- in the Create Key Pair dialog, insert a meaningful name for your key

- Click the "**+** Create Key Pair" button

![create-key-dialog](images/create-key-dialog.png)

- Your Public key is now registered in the list 

- and your Private key is now downloaded by your browser.

![1557213346498](images/registered-and-downloaded.png)
Your browser's default download folder is not an appropriate place to store your Private key. You should store your Private key in a suitably permanent place that is only accessible to you. 

- Create a folder for your Keys  in a suitably permanent place that is only accessible to you
- Move your downloaded Private key file into your new key folder.

PuTTY on Windows uses a slightly different Private key file format. If you are a Windows user and you intend to use PuTTY to ssh-connect to your instances, you will need to do a key conversion using PuTTYgen.

## ssh-keygen method
Duration: 4:00

## PuTTYgen method
Duration: 4:00



## PuTTYgen conversion

Duration: 5:00

Windows users that use PuTTY terminal software and have a Private key in `.pem`-format (e.g. from the Nectar Convenience method or `ssh-keygen`-method) will need to convert their Private key to `.ppk`-format. You can use PuTTYgen for the key conversion.

- If you don't yet have a copy of PuTTYgen, downoad it from the [PuTTY website](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html) 
- Launch PuTTYgen you can double click the `puttygen.exe` file
- Click 'Import key' item from the 'Conversions' menu:

![puttygen2](images/puttygen-conversions-import.png)

- Select the `.pem`private key you want to convert and click 'Ok'.
- Select 'Save private key' from the 'File' menu. 
- Click 'yes' to save your `.ppk`-key *without a passphrase*
- Save the converted private key using the same name as the original key file, but with the `.ppk`-extension

![puttygen](images/putty-file-save-private.png)

You are now ready use your Private key in `ppk`-format to `ssh`-connect using the PuTTY terminal software.

## Next Steps

positive
: **Cloud Starter**
Congratulations. You've completed one of the prerequisite steps for Launching a Virtual Machine in the Nectar Research Cloud. 
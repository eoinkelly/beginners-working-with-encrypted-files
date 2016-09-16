# Beginners guide for sending/receiving encrypted files on macOS

<!-- toc -->

- [Introduction](#introduction)
- [Overview of how encryption works](#overview-of-how-encryption-works)
- [Install GPG tools](#install-gpg-tools)
- [How to send your public key to somebody](#how-to-send-your-public-key-to-somebody)
- [What to do when you receive a public key](#what-to-do-when-you-receive-a-public-key)
- [Working with files](#working-with-files)
  * [How to encrypt a file](#how-to-encrypt-a-file)
  * [How to decrypt an encrypted file](#how-to-decrypt-an-encrypted-file)
  * [Extra Credit: Encrypt/decrypt text without having to create a file](#extra-credit-encryptdecrypt-text-without-having-to-create-a-file)

<!-- tocstop -->

## Introduction

## Overview of how encryption works

## Install GPG tools

Our first step to being able to confidently work with encrypted files is to download _GPG Tools_ from <https://gpgtools.org/>. _GPG Tools_ is a collection of tools that will integrate with macOS and let us encrypt and decrypt files.

Advanced users may enjoy knowing that _GPG Tools_ is a wrapper around [GnuPG](https://www.gnupg.org/). _GPG Tools_ installs _GnuPG_ (version `gpg (GnuPG/MacGPG2) 2.0.30` as of this writing) and it keeps your keys etc. in `$HOME/.gnupg` just as _GnuPG_ would. Less advanced users can sleep soundly knowing that they don't need to know any of that.

The installation of _GPG Tools_ is similar to many other macOS apps. Follow the prompts until we get to the screen asking you to "Generate a new key pair".

If you are confident installing macOS software you can skip straight ahead to the "Generate a key pair" screen. Otherwise you can see here a preview of you are likely to see during installation. Don't worry if what you see does not match these exactly (_GPG Tools_ may change their installer over time) - the important details will remain the same.

![GPG Suite dmg](./images/Screenshot 2016-09-16 13.24.44.png)
![GPG Installer Page 1](./images/Screenshot 2016-09-16 13.25.52.png)
![GPG Installer Page 2](./images/Screenshot 2016-09-16 13.26.00.png)
![GPG Installer Page 3](./images/Screenshot 2016-09-16 13.26.26.png)

The "Generate a new key pair" screen is important for us to understand. We are going to pause here to ensure we understand what is going on in this screen.

<!-- ![Generate new key pair 1](./images/Screenshot 2016-09-16 13.27.25.png) -->
![Generate new key pair detail](./images/Screenshot 2016-09-16 13.27.28.png)
![Generate new key pair detail and password filled in](./images/Screenshot 2016-09-16 13.28.14.png)
![GPG Tools generating key](./images/Screenshot 2016-09-16 13.28.31.png)
![Generate new key pair with advanced options visible](./images/Screenshot 2016-09-16 13.37.04.png)
![GPG Tools - main window with generated key](./images/Screenshot 2016-09-16 13.28.42.png)




## How to send your public key to somebody

If you want to email your public key to somebody there is a very fast way

1. Right-click on your keypair in the "GPG Keychain" window
1. Choose "Mail public key"
1. Your email software should open with a new email filled in with your public key as an attachment

If you want to save your public key as a file on your hard disks then

1. Right-click on your keypair in the "GPG Keychain" window
1. Choose export
1. Choose where to save the file
    * You can name the file anything you want but keep the `.asc` extension - this extension lets other encryption tools know that this file is for them i.e. it makes life easier for whoever you send/receive encrypted data with.
1. Make sure you do NOT tick the "Include secret key in exported file" - his is VERY IMPORTANT

![Export key dialog](./images/Screenshot 2016-09-16 14.37.59.png)

## What to do when you receive a public key

1 Double-click on the file your received - _GPG Tools_ should open and automatically import the key for you.

## Working with files

You can use _GPG Tools_ to encrypt files or pieces of text (from emails or chat messages).

To keep things simple we are going to focus on encrypting and decrypting files only.

If you do have a piece of text (from a chat or email) that you wish to encrypt or decrypt you should save it into a text file first e.g. using _TextEdit_ on macOS (show scr of textedit with encrypted content)

Check out our [Extra credit: encrypting/decrypting pieces of text]() section at the end if you regularly encrypt/decrypting pieces of text and want a faster workflow.

### How to encrypt a file

1. Save file on your local hard disk. If the encrypted message is part of an email or chat message copy and paste it into the TextEdit (show scr of both text edit and a chat window) and save that as a file first
1. Right-clic on file, go to Services menu and choose "OpenPGP Encrypt file"
1. Tick the public keys of everybody you want to send it to
1. also make sure the "Add to Recipients" is ticked so that it is also encrypted to your key

![Desktop with text file to encrypt](./images/Screenshot 2016-09-16 13.47.49.png)
![Encrypt file 1](./images/Screenshot 2016-09-16 13.47.29.png)
![Encrypt file 2](./images/Screenshot 2016-09-16 13.48.20.png)
![Encrypt file 3](./images/Screenshot 2016-09-16 13.48.44.png)
![Encrypt file 4](./images/Screenshot 2016-09-16 13.48.54.png)
![Encrypt file 5](./images/Screenshot 2016-09-16 13.49.11.png)

### How to decrypt an encrypted file

If the file is of the form `stuff.txt.gpg` just double-click it.

![Decrypt file 1](./images/Screenshot 2016-09-16 13.57.54.png)
![Decrypt file 2](./images/Screenshot 2016-09-16 13.58.09.png)
![Decrypt file 3](./images/Screenshot 2016-09-16 13.58.45.png)

### Extra Credit: Encrypt/decrypt text without having to create a file





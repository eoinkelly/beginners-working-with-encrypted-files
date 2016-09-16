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

then all your data is in ~/.gnupg
it also installs the command line tools

![GPG Suite dmg](./images/Screenshot 2016-09-16 13.24.44.png)
![GPG Installer Page 1](./images/Screenshot 2016-09-16 13.25.52.png)
![GPG Installer Page 2](./images/Screenshot 2016-09-16 13.26.00.png)
![Mac Password Prompt](./images/Screenshot 2016-09-16 13.26.15.png)
![GPG Installer Page 3](./images/Screenshot 2016-09-16 13.26.26.png)
![Generate new key pair 1](./images/Screenshot 2016-09-16 13.27.25.png)
![Generate new key pair detail](./images/Screenshot 2016-09-16 13.27.28.png)
![Generate new key pair detail and password filled in](./images/Screenshot 2016-09-16 13.28.14.png)
![GPG Tools generating key](./images/Screenshot 2016-09-16 13.28.31.png)
![GPG Tools - main window with generated key](./images/Screenshot 2016-09-16 13.28.42.png)
![Generate new key pair with advanced options visible](./images/Screenshot 2016-09-16 13.37.04.png)
![Desktop with text file to encrypt](./images/Screenshot 2016-09-16 13.47.49.png)

## How to send your public key to somebody

## What to do when you receive a public key

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





# Creating a Remote Server on DigitalOcean

## Introduction
In this tutorial, you will learn how to create a remote server using DigitalOcean. This tutorial will cover:
- Generating SSH Keys
- Adding a custom Arch Linux image
- Create a droplet running Arch Linux
- connecting to your droplet from your local machine using SSH
## SSH Keys
### What are SSH Keys
Secure Shell(SSH) keys are cryptographic keys that provide a secure connection between a device and server over an unsecured network. SSH uses encryption to scramble data which makes it more secure than a normal password.
### Steps to create a SSH Key
Make sure your device has ssh-keygen installed.
You may have to create a .ssh directory in your home directory. To create a .ssh directory in your home directory, run the command below
```powershell
`mkdir -p ~/.ssh`
```
To create a new SSH key pair, run the below command
```powershell
`ssh-keygen -t ed25519 -f ~/.ssh/do-key -C "your email address"`
```
This command creates a SSH key pair with a private and public key. The private key will be saved as "do-key" and the public key will be saved as "do-key.pub". The command will also associate your email with the key as a comment.

## Copy the contents of your SSH Public Key
For the next step, you will need to copy the contents of your SSH Public Key
Run the below command in your terminal

In PowerShell:
```powershell
`Get-Content C:\Users\your-user-name\.ssh\do-key.pub | Set-Clipboard`
```
For MacOS users:
``` 
pbcopy < ~/.ssh/do-key.pub
```
## Adding SSH Public Key to your DigitalOcean account
1. Log into your DigitalOcean account
2. Navigate to Settings > Security > SSH Keys
3. Click on add SSH Key
4. Paste the contents of your public key into the Public Key box and name it. 
## Adding a Custom Arch Linux image
1. Download a Arch linux image from 

## Creating a droplet running Arch Linux

## Connecting to your droplet
## References

SSH KEYS: https://www.cloudflare.com/learning/access-management/what-is-ssh/

SSH Key GITLAB CLass: https://gitlab.com/cit2420/2420-notes-f24/-/blob/main/2420-notes/week-two.md
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
## Adding a Custom Arch Linux image

## Creating a droplet running Arch Linux

## Connecting to your droplet
## References

SSH KEYS: https://www.cloudflare.com/learning/access-management/what-is-ssh/


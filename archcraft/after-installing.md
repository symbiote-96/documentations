# Things To Do After Installing Archcraft Distribution

As usual we need to prepare our OS to start working in it. For Archcraft we don't need to do much, this is because this distribution is so beautiful and so minimalist which is almost ready to work.

## First Updating The System

let's start with a system update.

> sudo pacman -Syuu

It happened to me that when I'm going to update my system, the output is some like this.

> error: archlinux-keyring: signature from "Christian Hesse <eworm@archlinux.org>" is unknown trust

We can solve this problem running the next command.

> sudo pacman -S archlinux-keyring && sudo pacman-key --populate

## Second, Git Configuration

For that we'll need to write these lines of code on our terminal.

> 1. git config --global user.name "John Doe"
>
> 2. git config --global user.email johndoe@example.com
>
> 3. git config --global core.editor vim
>
> 4. git config --global init.defaultBranch main
>
> 5. ssh-keygen -t ed25519 -C "your_email@example.com"
>
> - Note: If you are using a legacy system that doesn't support the Ed25519 algorithm, use:
>
> - ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

That is all. Finally we can check our changes with this command.

> git config --list

## Third, Install Visual Studio Code (vscode)

I know, I know. Some people could prefer to keep the system in its essence, minimalist, and use some editor like Neovim. But let's be practical. Everyone use vscode in the industry. If you decide to use vscode, run this.

> sudo pacman -S vscode

Now we have the basics. Check other documentations for more. 


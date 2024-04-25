# Research Software First Steps

Here are some steps you should take to enable collaborative CSE research with the group.

## Get important accounts

1. Sign up for a CU research commputing account (https://rcamp.rc.colorado.edu/accounts/account-request/create/organization). Google CU Reseach computing if link becomes out of date.

2. Create a GitHub account if you don't have one (https://github.com/join).

## Set up your local system

### Are you using a Windows Computer?
There are of course multiple ways to develop code on a windows machine but these steps are a good way to get started if you haven't used these tools before.

1. Install the Windows Subsystem for Linux (WSL) (https://learn.microsoft.com/en-us/windows/wsl/). This will allow you to use a similar unix based terminal as what is available on the cluster.
2. Install VSCode (https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode) and get it working with WSL.
3. Finally, follow these instructions to get git running on your home computer (https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-git)
4. Make sure you can clone the git repository for the project to your home computer.

### Are you using a Mac/Linux?

1. When using a Mac or Linux computer the terminal should make it easy to get git up and running using the built in terminal. Some instructions here (https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
2. Pick an editor. Again, there are unlimited options here but VS Code is available cross platform and is widely used.
3. Make sure you can clone the git repository for the project to your home computer.

## Get started on the research cluster

### Creating a Conda Environment to use with Jupyter notebooks

1. Follow instructions here to set up a jupyter python notebook using the interactive interface of Alpine. (https://curc.readthedocs.io/en/latest/gateways/OnDemand.html)
    1. It is generally best to store things in your project directory and, for posterity, in the repository for the project if possible (if files aren't too large or temporary).
    2. Conda installs packages by default in the home directory but the allotted space on the filesystem for the home directory is quite small on Alpine (2GB I think) so it is very easy to overrun that space with packages. One solution is to move the conda directory to your projects directory them create a symlink (basically an alias that redirects to another file) in your home directory. Just call these commands (each line separately) from the terminal (you don’t need to replace `$USER`). If this doesn't work, the install paths can also be modified in `.condarc`

        ```mv /home/$USER/.conda /projects/$USER/
        cd /home/$USER
        ln -sf /projects/$USER/.conda /home/$USER```

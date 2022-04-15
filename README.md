# MySQL-Tutorial

Based on [this video](https://youtu.be/8UT-oZzDW6c)



## Download MySQL
Download MySQL [here](https://dev.mysql.com/get/Downloads/MySQL-8.0/mysql-8.0.28-macos11-x86_64.dmg) or the latest DMG version (x86, 64-bit) [here](https://dev.mysql.com/downloads/mysql/)



## Password for the "root" user
In the "configuration" step of the installation, establish a password for the "root" user

<img width="400" alt="image" src="https://user-images.githubusercontent.com/65092569/163596060-55629278-cabc-4d71-a999-20f0061af1da.png">



## Start MySQL server
In "System Preferences" (on your computer), click on "Start MySQL server"

<img width="400" alt="image" src="https://user-images.githubusercontent.com/65092569/163597431-172041da-2889-493e-950a-51c25d0ceeaa.png">



## Use MySQL in Terminal

Press <kbd>CMD</kbd>+<kbd>SPACE</kbd> to open Spotlight Search

Search "/usr" and click on the "usr" folder

<img width="400" alt="image" src="https://user-images.githubusercontent.com/65092569/163598794-d1b8b45a-9afa-44d6-af5d-85047ed0714c.png">

There, go to "local/mysql-8.0.28-macos11-x86_64/bin and click on "Copy "bin" as pathname"

<img width="400" alt="image" src="https://user-images.githubusercontent.com/65092569/163598728-cbe310e9-bbd3-48de-9e74-2d59e6ac1b46.png">


Open the terminal and type: `open -t .zsh_profile`.

If you don't have that file:

Type `touch .zsh_profile` to create the .zsh_profile and `open -t .zsh_profile` to open the .zsh_profile file:

- On the file, paste `Export PATH=${PATH}:<your-path>` and save the file
- Now, reopen the Terminal and type `alias mysql=/usr/local/mysql/bin/mysql`

Then type `mysql --user=root -p`

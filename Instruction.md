# How to building with Flutter (in remote environment)

## Initial Setup
1. Fork the repo (important!)
2. Goto [GitPod](https://gitpod.io/)
3. Sign-in/up with your GitHub Account
4. Click on "New Workspace"
5. Select the repo you just created
6. Enter it
7. If there is any error pops up, don't worry and click on "X"

## You have to do these steps every time you open the Workspace
1. Click on the Sandwich on left upper corner
2. Terminal -> New Terminal
3. Copy&Paste in and hit enter

        flutter
4. If there is any error, great! continue the following steps
5. Copy&Paste in and hit enter

        cd ..
6. Copy&Paste in and hit enter

       git clone https://github.com/flutter/flutter.git -b stable
7. Copy&Paste and hit enter

        export PATH="$PATH:`pwd`/flutter/bin"
8. Type in hit Enter

        flutter doctor
    If still saying command not found, contact the tech support near you
9. Goto

        https://github.com/settings/emails
    If you **have Keep my email addresses private** and or **Block command line pushes that expose my email** enabled, you need set your email and username in the remote environment

        git config user.name "FIRST_NAME LAST_NAME"
        git config user.email "MY_NAME@example.com"
    Then check if its successful

        cat .git/config

## After the environemnt is ready
1. Type and ht Enter

        ls
2. Change Disk the the ? directory

        cd <?_directory>
    For example 

        cd Playground_Flutter
3. Change Disk the the project directory

        cd <project_directory>
    For example 

        cd app
4. CopyPasta and Enter

        flutter run -d web-server
    After loading for a while, it will show a link, Ctrl+LeftClick on that
        

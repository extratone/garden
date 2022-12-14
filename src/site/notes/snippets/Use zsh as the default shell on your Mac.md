---
{"dg-publish":true,"permalink":"/snippets/use-zsh-as-the-default-shell-on-your-mac/","dgHomeLink":true,"dgPassFrontmatter":false}
---

"Use zsh as the default shell on your Mac" | Apple Support

---
created: 2022-03-20T01:21:15Z
language: Markdown
modified: 2022-03-20T01:22:09Z
notes: [Use zsh as the default shell on your Mac - Apple Support](https://support.apple.com/en-us/HT208050)
tags: shell, macos, CLI
title: "Use zsh as the default shell on your Mac" | Apple Support
---

By default, your Mac uses either zsh or bash as the command-line interpreter for the login shell and interactive shell:

  * **zsh** (Z shell) is the default shell for all newly created user accounts, starting with macOS Catalina.
  * **bash** is the default shell in [macOS Mojave and earlier](https://support.apple.com/kb/HT201260).

zsh is highly compatible with the Bourne shell (sh) and mostly compatible with bash, with some differences. For more about zsh and its comprehensive command-line completion system, enter `man zsh` in Terminal.   

![](/library/content/dam/edam/applecare/images/en_US/mac_apps/itunes/divider.png)

## How to change your default shell

Whether your user account is configured to use zsh (recommended), bash, or another shell, you can change the default shell from Users & Groups preferences or the command line.

### From Users & Groups preferences

  1. Choose Apple menu  > System Preferences, then click Users & Groups. 
  2. Click the lock ![](/library/content/dam/edam/applecare/images/en_US/il/elcapitan-lock-inline.png), then enter your account name and password.
  3. Control-click your user name in the list of users on the left, then choose Advanced Options. 
  4. Choose a shell from the ”Login shell” menu, then click OK to save the changes.  


![](/library/content/dam/edam/applecare/images/en_US/macos/Mojave/macos-mojave-system-prefs-users-groups-advanced-login-shell.jpg)

### From the command line

In Terminal, enter `$ chsh -s path`, where path is one of the shell paths listed in /etc/shells, such as /bin/zsh, /bin/bash, /bin/csh, /bin/dash, /bin/ksh, /bin/sh, or /bin/tcsh.   

![](/library/content/dam/edam/applecare/images/en_US/mac_apps/itunes/divider.png)

## How to use a different shell without changing the default

If you don't want Terminal to use the default login shell in new Terminal windows and tabs:

  1. Open Terminal, then choose Terminal > Preferences.
  2. From the General pane, select ”Command (complete path).” 
  3. In the field provided, enter one of the shell paths listed in /etc/shells, such as /bin/zsh, /bin/bash, /bin/csh, /bin/dash, /bin/ksh, /bin/sh, or /bin/tcsh.

![](/library/content/dam/edam/applecare/images/en_US/macos/Mojave/macos-mojave-terminal-preferences-general-shells.jpg)

If you invoke the bash shell while macOS Catalina is configured to use a different shell, you'll see a message that the default interactive shell is now zsh. To silence this warning, you can add this command to ~/.bash_profile or ~/.profile: 
    
    
    export BASH_SILENCE_DEPRECATION_WARNING=1
    
    
    
    
    
    
    
                
            
    
    
    
        
            
    
    
        
    
        
                
                
    
    
    ![](/library/content/dam/edam/applecare/images/en_US/mac_apps/itunes/divider.png)
    
    
    
    
                
            
    
    
    
        
            
    
    
        
    
        
                
    
    ## How to switch to a zsh profile and prompt
    
    
                
    
    If you're using a bash profile, such as to set environment variables, aliases, or path variables, you should switch to using a zsh equivalent. For example:
    
    
    
    
    
    
      * **.zprofile** is equivalent to **.bash_profile** and runs at login, including over SSH
    
    
      * **.zshrc** is equivalent to **.bashrc** and runs for each new Terminal session
    
    
    
    
    If you're using **.profile** (a POSIX-compliant profile), you can make zsh automatically read its settings by adding this command to **.zprofile**:
    
    
    
    
    
    [[ -e ~/.profile | -e ~/.profile ]] && emulate sh -c 'source ~/.profile'
    
    
    
    
    
    You can also move some settings from a bash profile to a zsh profile without modification. For example, to set environment variables: export MY_SETTING=1.
    
    
    
    
    zsh recognizes a different set of prompt specifiers than bash and has a cleaner syntax for specifying colorized output, eliminating the need to use complex ANSI escape sequences. For example, here's the syntax for a default bash prompt from **.bash_profile**:
    
    
    
    
    
    export PS1="\[\e[92;40m\]\h\[\e[m\]:\[\e[93m\]\W\[\e[m\] \\$ "
    
    
    
    
    
    To convert that bash prompt to a zsh prompt when using **.zprofile** or **.zshrc**:
    
    
    
    
    
    export PS1="%10F%m%f:%11F%1~%f \$ "
    
    
    
    
    
    See the zsh man page for more details.
    
    
    
    
    
    
                
            
    
    
    
        
            
    
    
        
    
        
                
                
    
    
    ![](/library/content/dam/edam/applecare/images/en_US/mac_apps/itunes/divider.png)
    
    
    
    
                
            
    
    
    
        
            
    
    
        
    
        
                
    
    ## How to test your shell scripts
    
    
                
    
    To test script compatibility with Bourne-compatible shells in macOS Catalina, you can change /var/select/sh to /bin/bash, /bin/dash, or /bin/zsh. If you change /var/select/sh to a shell other than bash, be aware that scripts that make use of bashisms may not work properly.
    
    
    
    
    zsh can be made to emulate sh by executing the command zsh --emulate sh.
      
    
    
    
    
    
    
    
                
            
    
    
    
    
                                            
    
    
    

-"[Use zsh as the default shell on your Mac](https://support.apple.com/en-us/HT208050)"
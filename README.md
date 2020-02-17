---
title: Gatsby Code Profile 
---
# Gatsby Code Profile

This is a custom code profile built for [GatsbyJS](gatsbyjs.org) code Demos, it makes us a Gatsby color scheme and a variation of [Shades of Purple](https://marketplace.visualstudio.com/items?itemName=ahmadawais.shades-of-purple) created by [Ahmad Awais](https://marketplace.visualstudio.com/publishers/ahmadawais)

# What is a code profile ? 
A code profile is essentially a custom `settings.json` configuration that is shareable  and resuseable across different instances of VScode. It is mostly used to avoid repetition that comes with resetting the default `settings.json` of a VScode environment when you want to say, bump up the font-size for a screencast or feel like using a theme with other custom settings.  

> You can also customize which extensions load per code profile. 

# Setting up Gatsby_code_profiles

To set up the Gatbsy code profile you would have to follow these steps:

 1. Clone repository into your root directory .
 ```shell 
 git clone https://github.com/Ekwuno/gatsby_code_profiles.git
 ```
 Then change directory into the code profile.
 ```shell 
 git clone cd gatsby_code_profiles 
 ```
 In gatsby_code_profiles directory exists the presentation folder which houses the custom settings. 
 
 > Multiple sub folders can exist for code profiles and you would have to change directory to access the setting.
 
 
 2. Set up alias

Aliases are helpful for shortening commands and also help to reduce the cognitive load of learning a really long command and having to type it everytime. Vscode has a command line alias to [launch from the command line](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line) and this comes 
in handy.

For example, this repo lives in ~/gatsby_code_profiles and the command to launch my presentation settings and extensions is:

```code --extensions-dir ~/gatsby_code_profiles/presentation/exts --user-data-dir ~/gatsby_code_profiles/presentation/data```

The alias in the .zshrc file looks like this :

`alias gatsby-teach="code --extensions-dir ~/gatsby_code_profiles/presentation/exts --user-data-dir ~/gatsby_code_profiles/presentation/data"

> Now anytime you want to lunch VScode with the custom settings all you have to do it run gatsby-teach {name of directory}

# Lunching Profile


Restart your terminal and test out the command. You can include a project path to open it with that profile , or leave the directory blank to start a new project:
`gatsby-teach ./some-demo-directory`


### More profiles

As more profiles are added the Name of profile will aslo be updated 

`code --extensions-dir ~/gatsby_code_profiles/{Name of profile}/exts --user-data-dir ~/gatsby_code_profiles/presentation/data`

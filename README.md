# Gatsby Visual Studio Code Profile

This is a custom VS Code profile built for [Gatsby](gatsbyjs.org) code demos and docs, providing an accessible Gatsby color scheme. 

This theme is a variation of [Shades of Purple](https://marketplace.visualstudio.com/items?itemName=ahmadawais.shades-of-purple) created by [Ahmad Awais](https://marketplace.visualstudio.com/publishers/ahmadawais).

## What is a code profile? 

A code profile is a custom `settings.json` configuration that's shareable and reusable across different instances of VS Code. It is mostly used to avoid repetition that comes with resetting the default `settings.json` of a VS Code environment when you want to say, bump up the font-size for a screencast or feel like using a theme with other custom settings. 

For the Gatsby docs, a VS Code profile helps us create consistent learning materials.

## Setting up Gatsby_code_profiles

To set up the Gatsby code profile, follow these steps:

 1. Clone the repository **into your computer's root directory**.

 ```shell
 cd ~/
 git clone https://github.com/Ekwuno/gatsby_code_profiles.git
 ```
 Then change directories into the code profile.
 ```shell 
 cd gatsby_code_profiles 
 ```
 In the `gatsby_code_profiles` directory exists the presentation folder which houses the custom settings.  
 
 2. Set up an alias

To prevent from having to type a lengthy launch command every time, you'll want to set up an alias for your Terminal to launch VS Code with these settings and extensions from `~/gatsby_code_profiles`.

To set an alias for this command using [Oh My Zsh](https://ohmyz.sh/), paste this command into your `.zshrc` file:

```alias gatsby-teach="code --extensions-dir ~/gatsby_code_profiles/presentation/exts --user-data-dir ~/gatsby_code_profiles/presentation/data"```

> Now anytime you want to launch VS Code with the custom settings, you can run `gatsby-teach {name of directory}`.

## Launching the profile

Restart your terminal and test out the command. You can include a project path to open it with that profile, or leave the directory blank to start a new project:

```gatsby-teach ./some-demo-directory```

## Adding more profiles

As more VS Code profiles are added, the `Name of profile` will also be updated:

`code --extensions-dir ~/gatsby_code_profiles/{Name of profile}/exts --user-data-dir ~/gatsby_code_profiles/presentation/data`

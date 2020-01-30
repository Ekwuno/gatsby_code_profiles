# Setting up code-profiles

 - Clone repository (I recommed to your home directory)

Each folder in this repo represents one of those directories, which I refer to as "profiles" for lack of a better term.

> Right now we only have the presentation profile.

# Set up alias

Remembering the command to lunch the prfiles can bring a lot of cognitive load, so I used an alias in  my .zshrc.

For example, this repo lives in ~/gatsby_code_profiles and the command to launch my presentation settings is:

```code --extensions-dir ~/gatsby_code_profiles/presentation/exts --user-data-dir ~/gatsby_code_profiles/presentation/data```

The alias in my .zshrc looks like:

`alias gatsby-teach="code --extensions-dir ~/gatsby_code_profiles/presentation/exts --user-data-dir ~/gatsby_code_profiles/presentation/data"


# Lunching Profile


Restart your terminal and test out the command. You can include a project path to open it with that profile , or leave the directory blank to start a new project:
`gatsby-teach ./some-demo-directory`


### More profiles

As more profiles are added the Name of profile will aslo be updated 

`code --extensions-dir ~/gatsby_code_profiles/{Name of profile}/exts --user-data-dir ~/gatsby_code_profiles/presentation/data`

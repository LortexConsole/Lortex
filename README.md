# Table of items
- [Lortex](#lortex)
- [Lortex Script documentation](#lortex-script-documentation)
- [Building or installing](#building-or-installing)
- [License](#license)

# Lortex
Lortex is a console api made with nodejs to look like ubuntu
Lortex includes many features:
- sudo (Superuser)
- mkdir/rmdir/emptydir
- cd
- echo
- clear
- apt/apt-get (i made them the same)
- lortex-script (.ls files only works with js goto [Lortex Script Documentation](#lortex-script-documentation))
- lortex-profile (Parses .lortexprofile which is included into the dpc which is ~ "~/home/lortex-user")
- ls
- var
- exit
- execute
- execout

# lortex script documentation
Lortex Script is a instanceof json that has 3 vars
```json
{
  "execute.init": [], // execute.init the first thing that the lortex-script command looks at
  "execute.run": [], // execute.run only works when the lortex-script is in the middle if running the script file (after the init)
  "execute.end": [] // execute.end only works when the lortex-script command ends
}
```
Init/Run/End arrays only includes strings these strings are the commands which are runnable in console other commands it will return a error saying that the command not found

# Building or installing

You can fork the github page or download it or downloading a release.
After downloading the github page go inside and type "npm install".
After installing all packages do "npm run start".
And your done.

# License
Licensed under MIT license Check License file for all the license.

Creating a release for SharpGL is very straightforward. Ensure that you have installed all required pre-requisites (see [Developing SharpGL](https://github.com/dwmkerr/sharpgl/wiki/Developing-SharpGL)) and then move to the 'release' folder.

Run the command:

````
powershell.exe -f BuildRelease.ps1
````

All components of the project will be built, including Visual Studio Extenions and Nuget packages. The release will be stored in the 'release' folder under a folder with the version number.

This makes it very easy to quickly build a release if you are developing with SharpGL.
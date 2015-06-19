If you want to change SharpGL, debug it in detail or add new features, then have a quick read of this guide to get started with the development.

### Project Structure ###

SharpGL is actually composed of four solutions:

1. SharpGL
2. Samples
3. Tools
4. Extensions

The main SharpGL library code is in the SharpGL solution - this contains the core library and Scene Graph code. Each of the other solutions directly contain the core solution projects to ease debugging.

The Samples solution contains each of the samples for WPF and WinForms. The Tools solution contains some basic utilities and tools for working with SharpGL. SharpGL, Samples and Tools can be loaded and executed without any additional components.

The Extensions solution is used to build the Visual Studio Extensions (i.e. the project templates). This solution requires the Visual Studio SDK to be installed for the solution to open properly. You can get it here: [Visual Studio Software Development Kit](http://msdn.microsoft.com/en-us/library/bb166441.aspx).

### Pre-requisites ###

To build and develop the Visual Studio Extensions, you'll need the following components:

1. [Visual Studio 2010 SDK](http://www.microsoft.com/en-us/download/details.aspx?id=2680)
2. [Visual Studio 2012 SDK](http://www.microsoft.com/en-us/download/details.aspx?id=30668)

### Building a Release ###

To build a release, please follow the guide at [Creating a Release](https://github.com/dwmkerr/sharpgl/wiki/Creating-a-Release).
Running the SharpGL.vsix installer will add the SharpGL extensions to Visual Studio 2010. These extensions provide new project templates for creating SharpGL projects - for WinForms and WPF. The features provided by SharpGL.vsix are detailed on this page. To get the extension, go to the Downloads page, choose the latest download and download the 'SharpGL Visual Studio Extension' file.

## Installing the Extension

Download the SharpGL Core Binaries or SharpGL Visual Studio Extension package. Double click on the SharpGL.vsix file and you will be asked to confirm the installation of the extension:

![Installing the Extension](https://github.com/dwmkerr/sharpgl/blob/master/assets/wiki/img/extensions/ConfirmInstallation.png?raw=true)

This will install the SharpGL Extension.

## Using the WinForms Project Template

The first template installed is the WinForms project template.

Choose 'File > New > Project...' and from the list choose the 'SharpGL Windows Forms Application' template:

![New WinForms Project](https://github.com/dwmkerr/sharpgl/blob/master/assets/wiki/img/extensions/NewWinformsApplication.png?raw=true)

This template provides a WinForms application with an OpenGL control. The three main events of an OpenGL control are handled:

````csharp
private void openGLControl_OpenGLDraw(object sender, PaintEventArgs e)
{
    //  Get the OpenGL object.
    OpenGL gl = openGLControl.OpenGL;

    //  Clear the color and depth buffer.
    gl.Clear(OpenGL.GL_COLOR_BUFFER_BIT | OpenGL.GL_DEPTH_BUFFER_BIT);

    // ... etc ...
}

private void openGLControl_OpenGLInitialized(object sender, EventArgs e)
{
    //  TODO: Initialise OpenGL here.

    //  Get the OpenGL object.
    OpenGL gl = openGLControl.OpenGL;

    //  Set the clear color.
    gl.ClearColor(0, 0, 0, 0);
}

private void openGLControl_Resized(object sender, EventArgs e)
{
    //  TODO: Set the projection matrix here.

    //  Get the OpenGL object.
    OpenGL gl = openGLControl.OpenGL;

    //  Set the projection matrix.
    gl.MatrixMode(OpenGL.GL_PROJECTION);

    //  ...etc...
}
````

Running the application shows that the project renders a pyramid, performs a perspective projection transformation and initialises the clear color:

![WinForms App](https://github.com/dwmkerr/sharpgl/blob/master/assets/wiki/img/extensions/WinformsApp.png?raw=true)

This is a great starting point for your own OpenGL powered applications.

## Using the WPF Project Template

The second template installed is the WPF project template.

Choose 'File > New > Project...' and from the list choose the 'SharpGL WPF Application' template:

![New WPF App](https://github.com/dwmkerr/sharpgl/blob/master/assets/wiki/img/extensions/NewWpfApplication.png?raw=true)

This template provides a WPF application with an OpenGL control. The three main events of an OpenGL control are handled, Draw, Resize and Initialise. This is the perfect baseline for your own SharpGL WPF application. The default drawing routine creates a pyramid, as shown below:

![WPF App](https://github.com/dwmkerr/sharpgl/blob/master/assets/wiki/img/extensions/WpfApp.png?raw=true)

Other templates can be created if the community has a desire for them - if you would like to see more templates or different features, then please comment below or join in on the Discussions page.
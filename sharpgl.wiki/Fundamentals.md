This page details the most fundamental concepts of SharpGL that you must be aware of to begin developing applications.

## Naming Conventions ##

OpenGL constants are named in exactly the same way as they are in OpenGL and are constant members of the OpenGL class. As an example, the constants below:

````csharp
//  Two OpenGL constants.
GL_TRIANGLES
GLU_TESS_COMBINE
````

Would be written as:

````csharp
//  Two OpenGL constants.
OpenGL.GL_TRIANGLES
OpenGL.GLU_TESS_COMBINE
````

OpenGL functions are named in exactly the same way as they are in OpenGL - except that the 'gl' prefix is removed. For example, the calls below:

````csharp
//  Set the line width and point size.
glLineWidth(3.0f);
glPointSize(2.0f);
````

Would be written as:

````csharp
//  Get a reference to the OpenGL object.
OpenGL gl = openGLCtrl1.OpenGL;

//  Set the line width and point size.
gl.LineWidth(3.0f);
gl.PointSize(2.0f);
````

There is an exception to this rule. Parameter type postfixes are always removed from OpenGL function names. The appropriate function is called always based on the types used. For example, the calls below:

````csharp
//  Set the color.
glColor3f(0.5f, 0.5f, 0.5f);

//  Output some vertices.
glVertex3f(2.0f, 3.0f 4.0f);
glVertex4f(2.0f, 1.0f, 10.0f, 1.0f);
````

Would be written as:

````csharp
//  Set the color.
gl.Color3(0.5f, 0.5f, 0.5f);

//  Output some vertices.
gl.Vertex3(2.0f, 3.0f 4.0f);
gl.Vertex4(2.0f, 1.0f, 10.0f, 1.0f);
````

The number of parameters IS included at the end of the function name, just as it is in standard OpenGL calls. This is because in some cases, we still we need to know this - for example when calling glVertex3fv or glVertex4fv we need to know how many items in an array we are passing. Because of this, to maintain consistency if the OpenGL function has a number at the end of it, so does the SharpGL wrapper function.

## Calling OpenGL Functions ##

There are two different ways that OpenGL functions can be called.

**Direct OpenGL Calls**

You an use the OpenGL object directly to make OpenGL calls. Every function in OpenGL and all extension functions are included in the OpenGL object. All constants are also defined. In this case, a section of code as below:

````csharp
//  Set the polygon mode.
glPolygonMode(GL_FRONT, GL_FILL);
````

Would become:

````csharp
//  Get the OpenGL object.
OpenGL gl = openGLControl.OpenGL;

//  Set the polygon mode.
gl.PolygonMode(OpenGL.GL_FRONT, OpenGL.GL_FILL);
````

This is the most straightforward way to make OpenGL calls, and makes porting existing OpenGL code very simple.

**Direct OpenGL calls with Wrapped Enumerations**

Almost all OpenGL functions that take some kind of uint, such as glPolygonMode have overloads that provide enumerations as parameters. For example, the call below:

````csharp
//  Set the polygon mode.
glPolygonMode(GL_FRONT, GL_FILL);
````

Could be written as:

````csharp
//  Get the OpenGL object.
OpenGL gl = openGLControl.OpenGL;

//  Set the polygon mode.
gl.PolygonMode(PolygonFace.Front, PolygonMode.Fill);
````

This approach has the benefit that when you are writing the code, you have Intellisense to help you pick the appropriate parameter from the acceptable parameters only. However, this code is less alike standard OpenGL calls, so it may take more work to port existing calls to this style.

## Render Contexts ##

A Render Context is an object that manages the underlying Render Context Handle. Until a Render Context is created no OpenGL functions will work - and no extensions will be loaded. Calling OpenGL.Create will create the Render Context - once this is done extensions can be used but before this point they will not work.
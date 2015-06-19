SharpGL comes packaged with many sample applications to demonstrate key features or for you to use as starting points for your own development. This page is an index of the Sample Applications. Select any Sample Application to find out what it does, how it does it, and what it teaches you about SharpGL.

Please be aware that even though each sample is written either for WinForms or WPF, the techniques applied are perfectly valid for either.

### Modern OpenGL Sample (WinForms) ###

This sample shows how to use modern OpenGL features and reserved mode rendering. This sample is based on the [OpenGL 4.x tutorials](http://www.swiftless.com/opengl4tuts.html) on [Swiftless](http://www.swiftless.com/opengl4tuts.html).

![Thumbnail](https://github.com/dwmkerr/sharpgl/blob/master/assets/samples/ModernOpenGLSampleSmall.png?raw=true)

This sample shows how to use:

1. Simple pixel and fragment shaders.
2. Vertex Buffers
3. Custom matrices using [GlmNet](https://github.com/dwmkerr/glmnet). 

### Cel Shading Sample (WinForms) ###

This sample shows how to use modern OpenGL features and reserved mode rendering to draw a [Trefoil Knot](http://en.wikipedia.org/wiki/Trefoil_knot), either with simple per-pixel lighting or a [Cel Shading](http://en.wikipedia.org/wiki/Cel_shading) effect. The sample is based on the excellent article [Antialiased Cel Shading](http://prideout.net/blog/?p=22) from [The Little Grasshopper](http://prideout.net/blog/).

![Thumbnail](https://github.com/dwmkerr/sharpgl/blob/master/assets/samples/CelShadingSampleNormalSmall.png?raw=true)

This sample shows how to use:

1. Simple pixel and fragment shaders.
2. Cel shading
3. Anti-aliasing
4. Vertex Buffers
5. Vertex Buffer Arrays
6. Custom matrices using [GlmNet](https://github.com/dwmkerr/glmnet). 

## WinForms Samples


### Simple Drawing Sample

This basic sample shows how we can quickly create an application that uses SharpGL to render some geometry.

### Native Textures Sample

Want to add textures to your models? Here we see how the Scene Graph's Texture object can help us load texture data from image files, which you can then use in your applications.

### SharpGL Textures Sample

If you're using the Scene Graph Texture object, there's more you can do with Textures than just load them - in this sample we investigate more advanced functionality.

### Scene Sample

If you want to really unleash the power of the Scene Graph, you need a Scene. In this sample we create a Scene and show what can be done with it.

### Hit Test Sample

SharpGL can handle hit-testing for you - in this sample we find out how.

### Particle System Sample

Particle Systems are a great way to demo functionality - in this sample we create a simple Particle System.

### Polygon Loading Sample

Want to load geometry form *.obj or other files? No problem! In this sample we load some geometry from data files and display it in a Scene.

### Radial Blur Sample

In this sample we create a cool radial blur effect.

### Render Contexts Sample

Understanding how Render Contexts work is very useful - in this sample we demonstrate some of the different Render Contexts and look at how they compare to each other.

## WPF Samples

The WPF samples use the SharpGL, SharpGL.SceneGraph and SharpGL.WPF assemblies to demonstrate various features. They all use either the OpenGLControl or SceneView controls.

### Teapot Sample

The Utah Teapot is a classic for 3D applications - let's show how we can render it in a WPF application!

### Simple Shader Sample

Shaders are a powerful OpenGL feature, fully supported in SharpGL. In this sample we create, compile and use some simple shaders.

### Text Rendering Sample

Need to render 2D or 3D text? This sample shows you how you can do that!
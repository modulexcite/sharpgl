SharpGL supports almost all extensions and the core functionality of OpenGL to version 4.2. If you are unsure of whether an extension is supported, check here. If you find that an extension you need is not supported, please fork and add it or raise an issue.

## Core Functionality

All OpenGL Core Functionality is fully implemented up to and including: **OpenGL 4.2**

OpenGL Functions from 1.2 to 1.5 (inclusive) which have been deprecated in the standard are available to use, but marked as Obsolete - meaning that their usage will generate warnings.

## Supported Extensions

This page contains a list of OpenGL extensions organised by release. As each extension is incorporated into SharpGL, this page will be updated.

| Extensions                      | Extension ID           | Status          |
| ------------------------------- | ---------------------- | --------------- |
| OpenGL 1.1 Extensions                            
| Vertex Arrays                   | EXT_vertex_array       | Fully Supported |
| Polygon Offsets (Depth Biasing) | EXT_polygon_offset     | Fully Supported |
| RGBA logical blending           | EXT_blend_logic_op     | Fully Supported |
| Texture Copy and Sub-copy       | EXT_subtexture, EXT_copy_texture | Fully Supported |
| Texture Formats                 | EXT_texture            | Fully Supported |
| Texture Objects                 | EXT_texture_object     | Fully Supported |
| OpenGL 1.2 Extensions |
| 3D Volume Textures | GL_EXT_texture3D | Fully Supported | 
| BGRA Texture Format | GL_EXT_bgra | Fully Supported | 
| Packed Pixels | GL_EXT_packed_pixels | Fully Supported | 
| Normal Rescaling | GL_EXT_rescale_normal | Fully Supported | 
| Separate Specular Color | GL_EXT_separate_specular_color | Fully Supported | 
| Texture Coord Edge Clamping | SGIS_texture_edge_clamp | Fully Supported | 
| Texture LOD Control | SGIS_texture_lod | Fully Supported | 
| Draw Range Elements | EXT_draw_range_elements | Fully Supported | 
| Image Processing Subset | GL_SGI_color_table, GL_EXT_convolution, GL_SGI_color_matrix, GL_EXT_histogram, GL_EXT_blend_color, GL_EXT_blend_minmax | Fully Supported | 
| OpenGL 1.2.1 Extensions | 
| Multi-Texturing | GL_ARB_multitexture | Fully Supported | 
| OpenGL 1.3 Extensions | 
| Compressed Textures | GL_ARB_texture_compression | Fully Supported | 
| Cubemaps | GL_EXT_texture_cube_map | Fully Supported | 
| Multi-Sampling | GL_ARB_multisample | Fully Supported | 
| Texture Add | GL_ARB_texture_env_add | Fully Supported | 
| Texture Combine | GL_ARB_texture_env_combine | Fully Supported | 
| Texture Dot3 | GL_ARB_texture_env_dot3 | Fully Supported | 
| Texture Border Clamping | GL_ARB_texture_border_clamp | Fully Supported | 
| Matrix Transpose | GL_ARB_transpose_matrix | Fully Supported | 
| OpenGL 1.4 Extensions | 
| Automatic Mipmaps | SGIS_generate_mipmap | Fully Supported | 
| Blend Squaring Functions | GL_NV_blend_square | Fully Supported | 
| Depth Textures | GL_ARB_depth_texture | Fully Supported | 
| Hardware Shadowing Z-depth | GL_ARB_shadow | Fully Supported | 
| Fog Coordinates | GL_EXT_fog_coord | Fully Supported | 
| Multiple Draw Arrays | GL_EXT_multi_draw_arrays | Fully Supported | 
| Point Parameters | GL_ARB_point_parameter | Fully Supported | 
| Secondary Color | GL_EXT_secondary_color | Fully Supported | 
| Separate Blend Functions | GL_EXT_blend_func_separate | Fully Supported | 
| Stencil Wrapping | GL_EXT_stencil_wrap | Fully Supported | 
| Texture Crossbar Environment Mode | GL_ARB_texture_env_crossbar | Fully Supported | 
| Texture LOD Bias | GL_EXT_texture_lod_bias | Fully Supported | 
| Texture Mirrored Repeat | GL_ARB_texture_mirrored_repeat | Fully Supported | 
| Window Raster Position | GL_ARB_window_pos | Fully Supported | 
| OpenGL 1.5 Extensions | 
| VBOs Vertex Buffer Objects | GL_ARB_vertex_buffer_object | Fully Supported | 
| Occlusion Queries | GL_ARB_occlusion_query | Fully Supported | 
| Extended Shadow Functions | GL_EXT_shadow_funcs | Fully Supported | 
| OpenGL 2.0 Extensions | 
| Shader Objects | GL_ARB_shader_objects | Fully Supported | 
| Vertex Programs | GL_ARB_vertex_program | Fully Supported | 
| Vertex Shaders (VS) | GL_ARB_vertex_shader | Fully Supported | 
| Fragment Shaders (FS) | GL_ARB_fragment_shader | Fully Supported | 
| Multiple Render Targets | GL_ARB_draw_buffers | Fully Supported | 
| Non-power-of-two Texture | GL_ARB_texture_non_power_of_two | Fully Supported | 
| Rectangular Texture (limited subset of NPOT) | GL_ARB_texture_rectangle | Fully Supported | 
| Point Sprites | GL_ARB_point_sprite | Fully Supported | 
| Multiple Render Targets | GL_ARB_draw_buffers | Fully Supported | 
| Vertex texture fetch | GL_ARB_texture_float | Fully Supported | 
| Separate Blend Equation | GL_EXT_blend_equation_separate | Fully Supported | 
| Separate Stencil | GL_EXT_stencil_two_side | Fully Supported | 
| OpenGL 2.1 Extensions | 
| Non-Square Matricies | (glUniformMatrix) | Not Implemented | 
| PBOs Pixel Buffer Objects | GL_ARB_pixel_buffer_object | Fully Supported | 
| sRGB Texture (gamma 2.2) | GL_EXT_texture_sRGB | Fully Supported | 
| OpenGL 3.0 Extensions | 
| FBOs Frame Buffer Objects | GL_EXT_framebuffer_object | Fully Supported | 
| FBO Multisampling | GL_EXT_framebuffer_multisample | Fully Supported | 
| Hardware Instancing | GL_EXT_draw_instanced | Fully Supported | 
| VAOs Vertex Array Objects | GL_ARB_vertex_array_object | Fully Supported | 
| sRGB Framebuffers (gamma 2.2) | GL_EXT_framebuffer_sRGB | Fully Supported | 
| Transform Feedback | GL_EXT_transform_feedback | Fully Supported | 
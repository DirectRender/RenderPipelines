# OpenGL (1992)
> Pros
- OpenGL is a cross-platform graphics API, which means it can be used on a variety of platforms, including Windows, Mac OS, Linux, and embedded systems.
- OpenGL is fast and efficient. It is optimized for hardware acceleration and its code is highly optimized for performance.
- OpenGL is powerful and feature-rich. It includes a wide range of features for creating realistic 3D graphics, such as lighting, shading, textures, and shadows.
- OpenGL is easy to learn and use. There are many tutorials and resources available online to help developers learn the basics quickly.
> Cons
- OpenGL is not as popular as other graphics APIs, such as DirectX or Vulkan. Game Engines perfer DirectX or Vulkan over OpenGL.
- It does not have as many features as DirectX or Vulkan, which can make it more difficult to create complex 3D graphics.
- OpenGL is not as well supported by hardware manufacturers, which means that some hardware may not be able to support the latest features of OpenGL.
- The API is not as well documented as other graphics APIs, which can make it more difficult to learn and use.

# Vulkan (2016)
> Pros
- Vulkan is a low-overhead, cross-platform 3D graphics and compute API.
- Vulkan provides high performance with significantly reduced driver overhead.
- Vulkan simplifies parallel computation by providing tools for efficient multi-threaded rendering.
- Vulkan is supported on many platforms and devices, including Windows, Linux, Android, and iOS.
- Vulkan provides an easy-to-use interface that can be easily integrated with existing graphics engines and applications.
> Cons
- Vulkan requires a more complex setup than OpenGL.
- Vulkan may require additional hardware support for certain features.
- Vulkan may require additional development time and effort to integrate with existing codebases.
- Vulkan is a relatively new API, and so there is less community support and fewer resources available to help developers get up and running.


# DirectX (1995)
> Pros
- DirectX is designed to take advantage of the advanced hardware features found on modern graphics cards.
- DirectX allows developers to create more immersive and interactive gaming experiences, with realistic 3D visuals, dynamic lighting, and enhanced audio.
- DirectX includes a set of tools and libraries which make it easier for developers to create high-performance applications.
- DirectX is widely used in game development, allowing games to run on a variety of hardware configurations and still be able to use the same APIs.
> Cons
- DirectX can be difficult to learn due to its complexity.
- DirectX requires the use of specialized hardware, such as graphics cards, which can be expensive.
- DirectX is only available on Windows, limiting its use in cross-platform development.
- DirectX may not be supported by older hardware, and may not be compatible with certain software.




# What is a ``Shader``?
- Shaders is a program that is used to tell the graphics card how to display a certain object or scene. Shaders are responsible for the color, texture, and lighting of a 3D object or scene. They are written in a shading language such as Cg (C for graphics) or HLSL (High Level Shading Language) and are usually processed by the GPU.
- Shaders are run often on the GPU because they are designed to take advantage of the parallel processing capabilities of the GPU. Shaders can be used to perform a variety of tasks, including transforming and lighting 3D models, calculating reflections, generating shadows, and creating special effects. Some examples of shaders include vertex shaders, pixel shaders, geometry shaders, and compute shaders.

# What is a ``Vertex Buffer``?
- Vertex buffers are data structures used to store information about the vertices of a 3D model. A vertex buffer stores information like the position, color, and normal vector of each vertex in the model. This information is used by the graphics processing unit (GPU) to render the 3D model on the screen.
- Vertex buffer objects are used to store large collections of vertices on the graphics card for rendering. This allows the data to be quickly accessed by the GPU, which reduces the amount of time it takes to render a scene. Vertex buffer objects also reduce the amount of data that needs to be sent from the CPU to the GPU, which can improve performance in complex scenes.

# What is a ``Index Buffer``?
- Index buffers store the index data for a mesh, which specifies the order in which the vertices should be drawn. This can be used to reduce the amount of redundant vertex data and improve rendering performance.
- For example, consider a cube with eight vertices. If you were to draw the cube using a vertex buffer, you would need to specify all eight vertices in the buffer and then draw the cube by drawing two triangles for each face of the cube, for a total of 24 vertices. However, if you were to use an index buffer, you could specify just eight vertices in the vertex buffer and then use the index buffer to specify the order in which those vertices should be drawn, reducing the total number of vertices that need to be drawn.

# What is a ``Texture Buffer``?
- A texture buffer is a type of buffer in OpenGL that stores texture data. This data is typically stored in an image format, such as PNG or JPEG, and is used to add details and texture to a 3D model.

# What is a ``Uniform Buffer``?
- Uniform buffer is a type of buffer in OpenGL that stores uniform data. Uniform data is constant data that is the same for all vertices or fragments in a given draw call. This data is typically used to store transformations, lighting information, or other global data that needs to be shared across all the vertices or fragments in a scene

# What is a ``Shader Storage Buffer``?
- A shader storage buffer is a type of buffer in OpenGL that stores data that can be read and written by shaders. This allows shaders to interact with the graphics pipeline in more complex ways and perform more advanced computations on the GPU
- Shader storage buffers are useful for a variety of applications, such as creating complex particle systems, implementing GPGPU algorithms, or performing physics simulations. They allow you to store and manipulate data on the GPU using shaders, which can be much faster and more efficient than transferring data back and forth between the CPU and GPU.

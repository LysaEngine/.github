# Lysa Engine

Lysa Engine is a hobby 3D engine created for learning and experimenting with low-level graphics programming and game engine foundations.

## Features

- **Hybrid Rendering**: GPU-driven forward and deferred renderers.
- **Advanced Shaders & Post-processing**: Integrated with [Slang](https://shader-slang.org/) shaders.
  - **PBR**: Simplified Physically Based Rendering.
  - **Transparency**: Weighted Blended Order-Independent Transparency (OIT).
  - **Shadows**: Support for Directional and Point light shadow maps. Optional colored shadows for transparent objects.
  - **Culling**: GPU-driven Frustum Culling.
  - **Post-processing**: Bloom, SSAO, GTAO, FXAA, SMAA, TAA with optional frame sharpening, HDR Tone-mapping (Reinhard/ACES).
  - **Frame Scaling**: Bilinear filtering and AMD FSR with optional frame sharpening with AMD FSR RCAS.
  - **Physics Engine**: Integrated with [Jolt Physics](https://github.com/jrouwe/JoltPhysics) and [NVIDIA PhysX](https://nvidia-omniverse.github.io/PhysX/physx/5.6.1/index.html) for high-performance 3D physics.
  - **Collision Objects & Filtering**: Support for collisiion objects with object layer collision matrix.
  - **Raycasting**: Raycasting with layer-based filtering.
  - **Event Integration**: Physics contacts and collisions integrated with the engine's centralized event system.
  - **Debug Rendering**: Real-time visualization of physics shapes and constraints.
- **Core Systems**:
  - **Asynchronous Task Pool**: Multi-threaded task execution and deferred command buffering.
  - **Event System**: Centralized observer-based event dispatcher.
  - **Virtual File System**: Portable path resolution using `app://` URI schemes.
  - **Logging**: Flexible logging to console, file, or virtual debug window.
- **Resource Management**: Dedicated managers for Meshes, Textures, and Materials with automatic GPU uploading.
- **Modern C++**: Built with C++23, utilizing C++ modules for clean architecture.
- **Multi-API Support**: Vulkan and DirectX 12 support through [Vireo RHI](https://github.com/HenriMichelon/vireo_rhi).
- **Cross-Platform**: Designed for Windows (DirectX 12 & Vulkan), Linux (Vulkan) and potentially other platforms supporting Vulkan.
- **Scripting**: [Lua](https://lua.org/) bindings for high-level logic and rapid prototyping.
- **Editor**: Add-on to use Blender as an editor

## Getting Started

Please refer to the [Documentation](https://henrimichelon.github.io/Lysa/) for detailed instructions on how to integrate and build the engine in your project.

## Additional features

[Lysa Nodes](https://github.com/LysaEngine/lysa_nodes) is a scene graph system using OOP node tree for the Lysa Engine

[Lysa UI](https://github.com/LysaEngine/lysa_ui) is a user interface library designed specifically for the Lysa engine offering a hybrid system with retained-mode components drawn using an immediate mode vector renderer.

[Lysa ECS](https://github.com/LysaEngine/lysa_ecs) is an experimental ECS for the Lysa Engine using [Flecs](https://www.flecs.dev/flecs/)~~

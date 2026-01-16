# Lysa

Lysa is a hobby 3D engine created for learning and experimenting with low-level graphics programming and game engine foundations.

## Engine Features

- **Hybrid Rendering**: GPU-driven forward and deferred renderers.
- **Advanced Shaders & Post-processing**: Integrated with [Slang](https://shader-slang.org/) shaders.
    - **PBR**: Simplified Physically Based Rendering.
    - **Transparency**: Weighted Blended Order-Independent Transparency (OIT).
    - **Shadows**: Support for Directional and Point light shadow maps.
    - **Culling**: GPU-driven Frustum Culling.
    - **Post-processing**: Bloom, SSAO, FXAA, SMAA, and HDR Tone-mapping (Reinhard/ACES).
- **Core Systems**:
    - **Asynchronous Task Pool**: Multi-threaded task execution and deferred command buffering.
    - **Event System**: Centralized observer-based event dispatcher.
    - **Virtual File System**: Portable path resolution using `app://` URI schemes.
    - **Logging**: Flexible logging to console, file, or virtual debug window.
- **Resource Management**: Dedicated managers for Meshes, Textures, and Materials with automatic GPU uploading.
- **Modern C++**: Built with C++23, utilizing C++ modules for clean architecture.
- **Multi-API Support**: Vulkan and DirectX 12 support through [Vireo RHI](https://github.com/HenriMichelon/vireo_rhi).
- **Scripting**: [Lua](https://lua.org/) bindings for high-level logic and rapid prototyping.

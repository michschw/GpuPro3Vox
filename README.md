# GpuPro3Vox

This demo provides an **example implementation** of the voxelization algorithms presented in the [GPU Pro 3](https://www.routledge.com/GPU-PRO-3-Advanced-Rendering-Techniques/Engel/p/book/9781439887820) article "Practical Binary Surface and Solid Voxelization with Direct3D 11". Moreover, it showcases how to use the generated voxel data later on in a pixel shader, rendering the voxelization via a simple raycasting approach.

The demo is kept simple and is not optimized for performance; a few options can be controlled during runtime by the following keys:

| Key   | Action                                                      |
| ----- | ----------------------------------------------------------- |
| SPACE | Turn voxelization on/off (default: off)                     |
| TAB   | Display model or voxelization                               |
| 1     | Select rasterization-based surface voxelization             |
| 2     | Select rasterization-based solid voxelization               |
| 3     | Select conservative surface voxelization with DirectCompute |
| 4     | Select solid voxelization with DirectCompute                |
| L     | Toggle showing lines when displaying the voxelization       |

## Code

The code is largely identical to the original release accompanying the book. It was updated to replace dependencies that have become deprecated (such as the D3DX library) and to build with Visual Studio 2019.

Note that unlike the typical Direct3D application (in 2012), the demo adopts the OpenGL convention of a right-handed coordinate system and column vectors that are multiplied from the right to transformation matrices.

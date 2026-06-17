# android

## Purpose
Android integration library for SageLang. Enables development of Android apps with SageLang, featuring native GPU acceleration and composable UI support.

## Features
- **GPUContext**: High-level Vulkan/OpenGL ES abstraction.
- **Compose**: Sage-based UI composition layer.
- **Android Bridge**: Mapping SageLang constructs to native Android APIs.

## Usage Example
```sage
import android.app
import android.graphics

let gpu = GPUContext("My App")
let buf = gpu.create_buffer(1024, "storage")
gpu.upload(buf, [1.0, 2.0, 3.0, 4.0])
gpu.destroy()
```

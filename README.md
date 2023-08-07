# StarRailNPRShader

Fan-made shaders for Unity URP attempting to replicate the shading of Honkai: Star Rail. The shaders are not 100% accurate because this project is not a reverse engineering - what I do is to replicate the in-game looks to the best of my ability.

![my wife 1](/Sreenshots/silwolf.png)

<p align="center">↑↑↑ My Wife ↑↑↑</p>

![my wife 2](/Sreenshots/fuxuan.png)

<p align="center">↑↑↑ Also My Wife ↑↑↑</p>

## Requirements

- Unity 2022.3 (Recommended).
- Universal RP 14.0 or higher.
- My [ShaderUtilsForSRP](https://github.com/stalomeow/ShaderUtilsForSRP) package.
- Newtonsoft Json package 3.2.1 or higher (Optional).

## Extra features

Asset preprocess:

- Automatically smooth the normals of character models and store them into tangents. The file name of the model must match pattern `^Avatar_.+_00$`.
- Automatically process textures (if you haven't changed the file names after ripping them).

PostProcessing:

- Custom bloom using the method shared by Jack He in Unite 2018.
- Custom ACES tonemapping.

## Guide

- Use linear color space instead of gamma.
- HDR should be enabled.
- Depth priming must be disabled.
- Depth texture must be enabled and generated by a depth prepass.
- Rendering path must be forward currently.
- Renderer Feature `StarRailForward` must be added to the renderer.

## Special thanks

- miHoYo
- Related posts on Zhihu
- Related videos on bilibili
- °Nya°222

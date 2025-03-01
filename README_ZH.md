# ComfyUI 水印工具

[English](README.md)

该水印工具提供了一种即插即用的解决方案，使您能够在图像生成流程中嵌入自定义的水印信息。它可无缝集成到 ComfyUI 工作流中。项目中提供了适用于 stable 1.5、PixArt 以及 Flux 版本的示例工作流，展示了嵌入水印、生成图像以及提取水印的完整流程。

![Display](Display.png)

## 特性
- **易于集成：** 只需将此模块嵌入到您的 ComfyUI 工作流中即可使用。
- **即插即用：** 默认情况下，用户只需要修改水印 `message` 参数即可添加自定义水印。
- **完整流程：** 示例工作流包括水印嵌入、图像生成以及水印提取三个步骤。
- **多种实现：** 当前工具支持 Gaussian Shading (GS) 水印嵌入方法。

## 安装
进入 ComfyUI 目录 在终端或命令行中运行以下命令：
```
cd ComfyUI/custom_nodes/
```

添加 DPRW 节点 将包含 DPRW 节点的 Python 文件复制到 ComfyUI 的 custom_nodes 目录

```
git clone https://github.com/lthero-big/Comfyui-GaussianShadingWatermark.git
```

## 使用方法
1. **设置水印消息：**  
   在节点设置中编辑 `message` 参数，输入您希望嵌入的水印文字。
2. **嵌入水印：**  
   使用提供的节点将水印嵌入到潜在噪声中。
3. **生成图像：**  
   运行工作流，生成包含水印的图像。
4. **提取水印：**  
   使用水印提取节点验证或恢复图像中的水印信息。

## 示例工作流
项目中包含三个示例工作流：
- **MajicmixRealistic 版本：** 专为 Stable Diffusion 1.5 设计。
- **PixArt 版本：** 针对 PixArt 开发的工作流。
- **Flux 版本：** 适用于 Flux 的工作流。

只需加载并运行其中一个工作流，即可体验完整的水印嵌入、图像生成和水印提取过程。

**提取到的水印会在控制台显示**

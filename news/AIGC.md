## AIGC

1. DALL-E 3真的很擅长做贴纸设计。
    - 您可以一次生成一整包贴纸！ 这是提示：
        ```
        9 different stickers featuring [objects] with vibrant colors and white borders on a minimal background.
        （9 种不同的贴纸，以[物体]为特色，在最小的背景上具有鲜艳的色彩和白色边框。）
        ```
    - 3个额外提示：
        1. 有时贴纸边框是方形的。如果您希望围绕设计边缘切割边框，请在提示中添加"die cut"（“模切”）一词。
        2. 您可以在提示中显示多个对象。例如：
            - crazy ninja cats fighting chickens（疯狂的忍者猫打鸡）
            - christmas trees, reindeer, baubles and snowflakes（圣诞树、驯鹿、小玩意和雪花）
        3. 将它们变成WA贴纸：
            a. 使用 Clipdrop 删除背景。
            b. 剪掉每个贴纸。
            c. 使用免费工具，例如 WA Sticker Maker。
    - [图](https://wx2.sinaimg.cn/large/006af71Yly1hixfxk69mij30xc0xcn4e.jpg)

1. 感觉SD除了A1111客户端，也要玩一下comfyUI客户端才行——后者通过节点可视化“编程”的方式，对图像生成的控制已经精细到令人发指的程度！
        - 例如图中的两个case，是分别对3张参考图片分别选取了服饰、姿势和脸部特征进行混合，最后输出一张精确融合了上述特征的图片。
    - 解压即用安装包下载：github.com/comfyanonymous/ComfyUI
    - 汉化包链接（未测试）：github.com/taozuidesongshu/ComfyUI-to-Chinese
    - 案例出处：
        - https://twitter.com/NerdyRodent/status/1712870466644320583
    - [图](https://wx2.sinaimg.cn/large/7420b8eegy1hiwyb2f7sqj20xc0ltjvq.jpg)


1. 【#用DALL3和代码解释器制作GIF#】在DALLE 3中生成分割成块的逐帧图，然后用高级数据分析（原代码解释器）就能制作GIF了（作者：Nick Dobos） ​​​
    - [图](https://wx4.sinaimg.cn/large/006Fd7o3gy1hix6kks7o7j30wy106qj8.jpg)


1. 真实性惊人，谷歌、康奈尔提出真实的图像补全技术RealFill
    - 获得一张「完美」的图像，是 CV 研究人员长期以来努力的目标之一。日前，Google Research 和康奈尔大学的研究人员合作，提出了一种「真实的图像补全」（Authentic Image Completion）技术——用于图像补全的生成模型 RealFill。
    - RealFill 模型的优势是可以使用少量的场景参考图像进行个性化设置，而这些参考图像无须与目标图像对齐，甚至可以在视角、光线条件、相机光圈或图像风格等方面有极大的差异。一旦完成个性化设置，RealFill 就能够以忠实于原始场景的方式，用视觉上引人入胜的内容来补全目标图像。
    - 补画（inpainting）和扩画（outpainting）模型是能够在图像的未知区域生成高质量、合理的图像内容的技术，但这些模型生成的内容必然是不真实的，因为这些模型在真实场景的上下文信息方面存在不足。相比之下，RealFill 能够生成「应该」出现在那里的内容，从而使图像补全的结果更为真实。
    - 作者在论文中指出，他们定义了一个新的图像补全问题——「真实图像补全」（Authentic Image Completion）。不同于传统的生成型图像修复（替代缺失区域的内容可能与原始场景不一致），真实图像补全的目标是使补全的内容尽可能忠实于原始场景，用「应该出现在那里」的内容来补全目标图像，而不是用「可能在那里」的内容。
    - 论文链接：https://arxiv.org/abs/2309.16668
    - 项目页面：https://realfill.github.io/
    - [真实性惊人，谷歌、康奈尔提出真实的图像补全技术RealFill ​​​](https://mp.weixin.qq.com/s/j0_z_AoBnAHuom8d6pdwxg)
    - [图](https://mmbiz.qpic.cn/sz_mmbiz_png/KmXPKA19gWicJnm3xXU0tiboxmclLRtsBs0VWTwhCibt9jumB6lTbhZdibxoOJ60BiafiaoA96ZcSqUrLM1ghjewydvg/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)



1. stable diffusion原理解读通俗易懂，史诗级万字爆肝长文！ 
    - [stable diffusion原理解读通俗易懂，史诗级万字爆肝长文！ ](https://mp.weixin.qq.com/s/WbbotOH-awemHxSkw5X_Iw)


1. Dall-E 3 可以轻松为幻灯片或网站创建矢量插图。
    ```
        您不再需要在互联网上搜索图像，也不再有水印。
        它甚至可以免费与 Bing 或 ChatGPT Plus 配合使用。

        您可以按照以下步骤操作：
        1. 描述您想要的图像内容
        E.g.: "a professional man and woman chatting at a table with a presentation board behind them"
        （例如：“一对职业男女在桌边聊天，他们身后有演示板”）

        2. 将这些参数添加到提示中
        "flat simple vector illustrations style, vibrant colors, white background"
        （“平面简单矢量插图风格，鲜艳的色彩，白色背景”）

        这是我用来生成以下图像之一的完整提示的示例：

        提示→
        "A professional man and woman chatting at a table with a presentation board behind them, flat simple vector illustrations style, vibrant colors, white background"
        “一个职业男人和女人在桌边聊天，后面有演示板，平面简单矢量插图风格，鲜艳的色彩，白色背景”

        小提示：

        如果您想创建多个连贯的图像，可以添加颜色主题。

        只需在“白色背景”之前添加“blue theme"（蓝色主题）即可。
    ```






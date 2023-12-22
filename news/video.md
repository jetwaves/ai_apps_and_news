## 视频

1. 文字生成视频的AI产品Runway Gen-2
    - 这次更新有点强啊，画面质量提升巨大，从稳定性到分辨率都非常精美了


1. 下载youtube视频的方法：
    ```
        yt-dlp 只能下载完整视频，不支持下载指定视频的时间段。而 ffmpeg 可以从输入的视频中截取指定时间段，即使输入的视频是网络链接而非本地文件。

        yt-dlp 加上 -g 参数可以只打印出视频下载链接而不下载视频。所以，可以把 yt-dlp -g 的输出作为 ffmpeg 的输入，结合 yt-dlp 和 ffmpeg 实现下载网络视频中指定的一段。

        不过不是所有视频格式都能用这种方式。对于 youtube 来说，至少格式 22（720p 的 h264 视频 + AAC 音频）、格式 137（1080p 的 h264 视频）、格式 140（AAC 音频）是可以的。

        如果要下载 720p 的，只需要一行命令：
        ffmpeg -copyts -ss 00:17:51 -to 00:18:56 -i $(yt-dlp -g mULUDboJnB0 -f 22) -c copy 22.mp4

        如果要下载 1080p 的，需要分别下载音频和视频，然后合并：
        ffmpeg -copyts -ss 00:17:51 -to 00:18:56 -i $(yt-dlp -g mULUDboJnB0 -f 137) -c copy 137.mp4
        ffmpeg -copyts -ss 00:17:51 -to 00:18:56 -i $(yt-dlp -g mULUDboJnB0 -f 140) -c copy 140.m4a
        ffmpeg -i 137.mp4 -i 140.m4a -c copy 137+140.mp4
    ```

1. VideoCrafter: 转自歸藏（twitter.com/op7418）：
    - 腾讯和香港科技大学一起开源了一个新的视频生成模型。
        - 其中包括视频VAE和3D去噪U-net。在2000万个视频和6亿张图像上进行训练，优于其他开源视频生成模型。
        - 这是一个类似与 pika 和moonvalley 的技术，他们还开放了一个类似的 Discord 频道用来测试。支持图片生成视频和文字生成视频。感兴趣可以去试试。
    - 原推文：twitter.com/op7418/status/1719261493278220526
    - 项目首页：ailab-cvc.github.io/videocrafter/
    - 代码库：github.com/AILab-CVC/VideoCrafter
    - [预览图](https://ailab-cvc.github.io/videocrafter/img/overall.jpg)

1. VideoReTalking，根据输入视频和声音生成相匹配的新视频↓
    - 项目主页：github.com/OpenTalker/video-retalking
    - Demo：opentalker.github.io/video-retalking
    - 在线体验：colab.research.google.com/github/vinthony/video-retalking/blob/main/quick_demo.ipynb
    - 摘要：
        - 我们推出了 VideoReTalking，这是一种新系统，可根据输入音频编辑现实世界中头部说话视频的脸部，即使具有不同的情绪，也能生成高质量且口型同步的输出视频。
        - 我们的系统将这一目标分解为三个连续的任务：
            - 具有规范表达的人脸视频生成；
            - 音频驱动的口型同步；
            - 面部增强以提高照片真实感。
        - 给定一个头部说话的视频，我们首先使用表情编辑网络根据相同的表情模板修改每一帧的表情，从而产生具有规范表情的视频。然后将该视频与给定的音频一起输入到口型同步网络以生成口型同步视频。最后，我们通过身份感知面部增强网络和后处理来提高合成面部的照片真实感。
        - 我们对所有三个步骤都使用基于学习的方法，并且我们的所有模块都可以在顺序管道中处理，无需任何用户干预。
    - 视频：https://video.weibo.com/show?fid=1034:4960884141785155

1. ProPainter：改进视频修复的传播和转换器
    - 来自南洋理工大学的这个厉害了！
    - 可以把视频里的人给抠干净，且抠完人后还能自动修复（恢复）背景
    - github.com/sczhou/ProPainter
    - [视频](https://video.weibo.com/show?fid=1034:4955568943857668)








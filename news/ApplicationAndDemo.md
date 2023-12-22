## demo和案例

1. #实时图像扩散效果#，基于潜在一致性模型实现。
    - 参考链接：https://huggingface.co/spaces/radames/Real-Time-Latent-Consistency-Model
    - 视频：https://video.weibo.com/show?fid=1034:4962559875285070

1. 具有 3D 预览功能的购物APP程序演示
    - 使用了 Reanimated（React Native的动画库） 和 ThreeJS ，该应用提供了一种3D预览功能，让用户能够更直观地查看商店中的商品。
    - GitHub：github.com/alexandrius/react-native_3d_store 
    - 视频：https://video.weibo.com/show?fid=1034:4962492288270365

1. 这个视频厉害了！在任何一点暂停，它都会看起来像一个正常的风景！
    - 作者描述的制作过程：
        - 使用 FFmpeg 等工具将视频分割成帧。使用简单的描述进行提示，例如“令人惊叹的风景的获奖照片”，并添加负面提示以避免不良输出。使用 ControlNet QR-Code Monster 1.5 倍强度或更高。选择批处理图像并输入框架文件夹的路径，而不是单个图像。对每一帧使用相同的种子可以提供更好的一致性。然后，将帧重新组合成视频并添加回音频。
    - 所需时间取决于目标分辨率、帧速率和视频长度。在 512x608 分辨率下，在 RTX 4090 上完成 5300 帧大约需要 4 小时。在 1308x1020 分辨率下（如上传的压缩视频所示），需要 14 小时。
    - 视频：https://video.weibo.com/show?fid=1034:4961164904562748


1. 游泳运动员徐佳玲使用大脑控制的智能仿生手，点燃了亚残运会的主火炬塔
    - 动图：https://wx3.sinaimg.cn/large/007Qt9CBly1hj7eu0317gg30a00hsnpq.gif

1. 网友Gorden Sun（twitter.com/gorden_sun）用HeyGen生成的效果，上传了一段英文视频，然后HeyGen自动翻译、配音，最后合成新的视频，口型、卡点和嘴型都对的上。
    - 但这个目前也有限制：你不能提供自己的翻译，只能是HeyGen自动帮你翻译，所以有时候翻译的效果会很生硬。
    - 原文：twitter.com/gorden_sun/status/1716075577117929841
    - ![图](https://wx1.sinaimg.cn/large/66fd066bgy1hj4hsurpsjj20xi1aq1gj.jpg)
    - 视频：https://video.weibo.com/show?fid=1034:4959795644661777


1. 这是用supervision构建的最令人兴奋的项目之一↓
    - Vriza Wahyu Saputra 使用supervision API 中提供的移动 LineZone，构建了这个精彩的球杂耍计数演示。
    - 代码：github.com/roboflow/supervision
    - 视频： https://video.weibo.com/show?fid=1034:4957595426029635


1. AI技术，可让WiFi信号成为摄像头。
    - 被技术接管的人类社会，已经成型。 大家都是这个人类动物园中的裸猿！
    - 视频： https://video.weibo.com/show?fid=1034:4957084471459916
















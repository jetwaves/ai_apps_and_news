## 声音相关应用

1. XTTS：这是一个声音克隆项目，只要几秒钟的音频样本就能创造出 AI 语音克隆。刚刚的发布了 XTTS v2，
   - 包括以下重要更新：
     - 更出色的零样本克隆能力
     - 可以用更多数据进行克隆
     - 更加自然的语调和表达力
   - 项目地址：github.com/coqui-ai/tts
   - HuggingFace 上的测试地址：https://huggingface.co/coqui/XTTS-v2


1. Voice Changer 是一款实时语音转换客户端，支持Windows和Mac。
    - 它可以实时变声成其他人或者虚拟角色的音色，可以接入多种语音转换技术，例如：
      - MMVC（github.com/isletennos/MMVC_Trainer）
      - so-vits-svc （github.com/svc-develop-team/so-vits-svc）
      - RVC(Retrieval-based-Voice-Conversion) （github.com/liujing04/Retrieval-based-Voice-Conversion-WebUI）
      - DDSP-SVC （github.com/yxlllc/DDSP-SVC）
    - 对于如何使用，有一个YouTube教学视频讲的蛮详细：www.youtube.com/watch?v=_JXbvSTGPoo
    - 项目地址：github.com/w-okada/voice-changer
    - [图](https://wx4.sinaimg.cn/large/66fd066bgy1hj3l4ssth0j20lg07ydik.jpg)

1. VideoReTalking：让视频中的人物的嘴型与输入的声音同步。
  - 你只需要输入任意一个视频和一个音频文件，它能给你生成一个新的视频，在这个视频里，人物的嘴型会与音频同步。VideoReTalking不仅可以让嘴型与声音同步，还可以根据声音改变视频中人物的表情。整个过程不需要用户干预，都是自动完成的。
  - 工作流程：
    - 整个系统的工作流程分为三个主要步骤：面部视频生成、音频驱动的嘴型同步和面部增强。所有这些步骤都是基于学习的方法，并且可以在一个顺序的流程中完成，无需用户干预。
      1. 面部视频生成：首先，系统会使用表情编辑网络来修改每一帧的表情，使其与一个标准表情模板相符，从而生成一个具有标准表情的视频。
      2. 音频驱动的嘴型同步：然后，这个视频和给定的音频一起被输入到嘴型同步网络中，生成一个嘴型与音频同步的视频。
      3. 面部增强：最后，系统通过身份感知的面部增强网络和后处理来提高合成面部的照片真实性。
  - 该系统是使用 PyTorch 实现的，并且每个模块都是单独训练的。系统在 VoxCeleb 数据集上进行了训练。
    - VoxCeleb 是一个大型的、多样性丰富的说话头部视频数据集。这个数据集包含了 22,496 个不同身份和头部姿态的说话头部视频。选择这个数据集的目的是为了确保模型能够处理各种各样的说话头部视频。
    - 通过这样详细和精细的训练过程，VideoReTalking 成功地实现了一个能够生成高质量、嘴型与音频同步的说话头部视频编辑系统
  - 项目及演示：opentalker.github.io/video-retalking/
    - 论文：arxiv.org/abs/2211.14758
    - GitHub：github.com/OpenTalker/video-retalking
    - Colab在线体验：colab.research.google.com/github/vinthony/video-retalking/blob/main/quick_demo.ipynb


1. 张鑫旭新文章：“纯JS实现多个音频的拼接或者合并” 
  - https://www.zhangxinxu.com/wordpress/2023/10/js-audio-audiobuffer-concat-merge/
  - 3年前有更新过JS剪裁audio音频，今天我们再讲讲如何使用原生的JS实现多个音频的拼接或合并，此文可是其他地方见不到的哟。 ​​​


1. lalal.ai，这个音频处理工具太牛了，它可以对复杂的合成音轨进行精准分离和无损提取。我试了一下，效果非常好。
  - 它主要用于两个场景，一个是音轨剥离，一个是声音移除，例如它可以提取人声、鼓、贝斯、吉他和弦乐等声音，也可以去除背景音乐、麦克风隆隆声以及其他不需要的噪音。
  - 下面的视频演示了剥离伴奏和人声的效果，还是比较直观的。
    - https://video.weibo.com/show?fid=1034:4954729168437260
  - 也去搜罗了下实现原理，找到一篇介绍 MSS（Musical Source Separation）的论文：
    - inria.hal.science/hal-01945345/document，
    - 它介绍了基于模型和基于信号处理的两种较为传统的处理方式，也提到，当前引入深度神经网络来解决这个问题的应用越来越多，不过最大的局限性还是可用于学习的数据太少，例如你让工具单独提取音频中鸟叫的声音，可能就比较吃力。





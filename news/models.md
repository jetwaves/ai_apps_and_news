
## AI模型
2023/09/24
1. 三秒语音就能克隆自己的声音，VALL-E-X本地部署与使用教程，开源免费，支持中文
    - 教程： https://www.youtube.com/watch?v=D8tFRIF92WY

1. 开源最彻底的大模型来了——130亿参数，无需申请即可商用。不仅如此，它还附带着把全球最大之一的中文数据集也一并开源了出来：600G、1500亿tokens！
    - 这就是来自昆仑万维的Skywork-13B系列，包含两大版本：
        - Skywork-13B-Base：该系列的基础模型，在多种基准评测中都拔得头筹的那种。
        - Skywork-13B-Math：该系列的数学模型，数学能力在GSM8K评测上得分第一。
    - 在各大权威评测benchmark上，如C-Eval、MMLU、CMMLU、GSM8K，可以看到Skywork-13B在中文开源模型中处于前列，在同等参数规模下为最优水平。
        - 而Skywork-13B系列之所以能取得如此亮眼的成绩，部分原因离不开刚才我们提到的数据集。
        - 毕竟清洗好的中文数据对于大模型来说可谓是至关重要，几乎从某种程度上决定了其性能。
        - 但昆仑万维能将如此“至宝”无偿地给奉献出来，不难看出它对于构建开源社区、服务开发者的满满诚意。
    - 除此之外，昆仑万维Skywork-13B此次还配套了“轻量版”大模型，是在消费级显卡中就能部署和推理的那种！
    - Skywork-13B下载地址（Model Scope）：
        - https://modelscope.cn/organization/skywork
    - Skywork-13B下载地址（Github）：
        - https: //github.com/SkyworkAI/Skywork
    - 接下来，我们进一步来看下Skywork-13B系列更多的能力。
        - [原文](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247701790&idx=2&sn=0153f07934600533024ea94467a4fb07&chksm=e8df626cdfa8eb7a44290ab10a9b608a390166bdce24c138a4e39227e2e94128333d62613eb5&token=1055698904&lang=zh_CN#rd)
    - [图:模型排名](https://mmbiz.qpic.cn/mmbiz_png/YicUhk5aAGtAtaxJbgYmPT9hU980OQLsLfT5oXpzY9JyCM0ibrJu5s6kCkZh00BXHlFIugfw00QYllXsUZnvptUQ/640?wx_fmt=png&wxfrom=5&wx_lazy=1&wx_co=1)



1. 来自“欧洲OpenAI”的“最强7B开源模型”Mistral最近可谓是圈粉无数。
    - 来自法国的开源大模型Mistral-7B成开源社区新宠，Llama 2都不香了。
        - 它各方面的测试指标全面超越了13B的Llama2，甚至让一众网友觉得羊驼不香了。
        - 67%的人选择基于它创业而不是Llama 2
        - 发布不到2周，配套生态也迅速发展起来，如何在单卡上微调的教程有了。
        - 各种基础设施和工具链也添加了对Mistral-7B的支持。
        - 与Meta刚刚发布Llama的时候，迅速出现各种其他驼和神兽，发展成大模型动物园的场景太像了。
    - 为什么Mistral这么火？
        - 性能更强，7B在所有benchmark超过llama 2 13B。
        - 硬件需求更少，笔记本轻松跑，量化后只需要6G显存。
        - 训练数据新，有2023年的知识。
        - 实用性更高，安全对齐没那么离谱，不会拒绝回答“如何杀死一个Linux进程”。
        - 开源协议更宽松，Apache2.0。
    - 最新消息是，Mistral AI团队已经发布了相关论文，透露背后的技术细节。
    - [“最强7B模型”论文发布，揭秘如何超越13B版Llama 2 ​​​](https://zhuanlan.zhihu.com/p/661113652)
    - 论文地址：https://arxiv.org/abs/2310.06825
    - 微调教程：https://wandb.ai/byyoung3/ml-news/reports/Fine-Tuning-Mistral7B-on-Python-Code-With-A-Single-GPU---Vmlldzo1NTg0NzY5





















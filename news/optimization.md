## 优化

1. RAG 很热！
    - 每个人都在谈论的一个话题是检索增强生成（RAG），它是一种框架，用于通过将模型建立在外部知识源的基础上来提高大型语言模型生成文本的质量。它本质上是一种使用企业或用户特定的数据来训练模型并帮助模型“查找”外部信息以改进其响应的技术。RAG 与微调不同，微调是采用预先训练的 LLM 并在较小的特定数据集上对其进行进一步训练，以使其适应特定任务或提高其性能的过程。
    - RAG 无疑正在迎来它的辉煌时刻。在关于构建生成应用程序的新兴架构的小组中，LangChain 的 Harrison、Unstructed 的 Brian 和 OctoML 的 Luis 讨论了 RAG 的优缺点以及它在 AI 开发人员中日益流行，特别是因为它比微调更便宜，而且更多可以概括的。另一个讨论主题是培训法学硕士，然后根据特定用例使用另一个法学硕士进行重新培训的能力。
    - 显然，目前还没有明确的标准。各种规模的公司都在将几种不同的技术结合在一起来优化模型性能。


1. NVIDIA的Stable-Diffusion加速插件 Stable-Diffusion-WebUI-TensorRT 微博正文 的图像生成加速。 
    - 速度确实很快，但由于速度优先，质量有所下降。
    - https://twitter.com/Yokohara_h/status/1714677568023285840

1. 【PyTorch官方认可！斯坦福博士新作：#长上下文LLM推理速度提8倍#】
    ```
        这两天，FlashAttention团队推出了新作：
        一种给Transformer架构大模型推理加速的新方法，最高可提速8倍。

        该方法尤其造福于长上下文LLM，在64k长度的CodeLlama-34B上通过了验证。
        甚至得到了PyTorch官方认可。

        如果你之前有所关注，就会记得用FlashAttention给大模型加速效果真的很惊艳。
        不过它仅限于训练阶段。

        因此，这一新成果一出，就有网友表示：
        等推理加速等了好久，终于来了。

        据介绍，这个新方法也是在FlashAttention的基础之上衍生而出，主要思想也不复杂：
        用并行操作尽快加载Key和Value缓存，然后分别重新缩放再合并结果，最终获得推理速度上的大幅提升。
    ```
    - 详细来看: 知乎专栏：https://zhuanlan.zhihu.com/p/661801492
    - 官方博客：https://princeton-nlp.github.io/flash-decoding/
    - 参考链接：https://twitter.com/tri_dao/sta
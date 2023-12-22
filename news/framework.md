## 框架

1. 微软研发的 AutoGen 框架太强大了，它是一个多代理框架，利用它可以轻松定制一系列工作任务。h++ps://github.com/microsoft/autogen
    - 举一个常见的例子：我们要实现一个爬虫程序，抓取并保存网页图片。如果把这个任务丢给 ChatGPT，它会直接返回一串可执行代码，但是代码通常会存在问题，例如执行报错、缺少依赖等，你需要反复跟 ChatGPT 对话来完善程序。当然，我们也可以设定一个复杂 Prompt，要求它调用 ChatGPT 的代码执行插件，如果存在报错，则继续修正程序。
    - 这个任务如果交给 AutoGen 来实现，将会变得无比简单，几行代码就可以搞定：
        1. 定义一个 Assistant Agent，它的任务是解决问题
        2. 定义一个 UserProxy Agent，它的任务是替代人询问问题，同时在本地执行程序
    - 这两个 Agent 都不需要给他们设置 Prompt。当我们把爬虫任务交给 UserProxy 后，它会理解任务，然后询问 Assistant 应该如何做，Assistant 会把操作过程告诉 UserProxy，接着 UserProxy 会根据指示在本地安装依赖，然后创建文件执行代码，如果执行出现错误，它会把详细报错提交给 Assistant，依次循环，直到可以获取到最终的结果。任务结束的时候，你会看到目标图片已经保存到本地磁盘了。
    - 利用这个框架可以做的事情非常多，它提供的能力也十分完善，可以在项目的 notebook 中找到很多最佳实践：h++ps://github.com/microsoft/autogen/tree/main/notebook
    - P.S. 为了确保安全，还是建议你在 Docker 环境中执行程序，UserProxy 有一个 code_execution_config 配置，将 use_docker 配置为 True 即可；另外，它还有一个 human_input_mode 参数，设置为 NEVER，表示整个过程都不需要人参与，也可以设置为其他值，它会等待人的输入后再进行下一步操作，这个设计可以让人参与到任务执行过程，避免跑偏。
    - [视频](https://video.weibo.com/show?fid=1034:4956079881125938)






















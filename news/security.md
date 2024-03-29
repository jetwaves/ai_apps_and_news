
## 安全
2023/09/16
1. GitHub 上一款简单易用、广受好评的 Web 防火墙工具：雷池 WAF，可保护你的网站不受黑客攻击。
    - 底层基于 Nginx 的 Web 网关，采用业界领先的语义引擎检测技术，作为反向代理接入网络，清洗来自黑客的恶意流量。
    - 项目安装简单便捷，采用容器化部署，一条命令即可完成安装，0 成本上手。
    - 借助智能语义分析算法，实现精准检测、低误报、难绕过，面对未知特征的 0day 攻击不再手足无措。
    - 无规则引擎，线性安全检测算法，平均请求检测延迟在 1 毫秒级别。并发能力强，单核轻松检测 2000+ TPS，只要硬件足够强，可支撑的流量规模无上限。
    - GitHub：github.com/chaitin/safeline


1. 1分钟不到、20步以内“越狱”任意大模型，绕过安全限制！
    ```
        而且不必知道模型内部细节，只需要两个黑盒模型互动，就能让AI全自动攻陷AI，说出危险内容【图1】。

        听说曾经红极一时的“奶奶漏洞”已经被修复了:【图2】。那么现在搬出“侦探漏洞”、“冒险家漏洞”、“作家漏洞”，AI又该如何应对？【图3】
        一波猛攻下来，GPT-4也遭不住，直接说出要给供水系统投毒只要……这样那样。
        关键这只是宾夕法尼亚大学研究团队晒出的一小波漏洞，而用上他们最新开发的算法，AI可以自动生成各种攻击提示。

        研究人员表示，这种方法相比于现有的GCG等基于token的攻击方法，效率提高了5个量级。而且生成的攻击可解释性强，谁都能看懂，还能迁移到其它模型。无论是开源模型还是闭源模型，GPT-3.5、GPT-4、 Vicuna（Llama 2变种）、PaLM-2等，一个都跑不掉。

        成功率可达60-100%，拿下新SOTA。

        话说，这种对话模式好像有些似曾相识。多年前的初代AI，20个问题之内就能破解人类脑中想的是什么对象。
        如今轮到AI来破解AI了。
    ```
    - [20步内越狱任意大模型！更多“奶奶漏洞”全自动发现](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247702557&idx=3&sn=48c0e6fed8b984781142956757944fed&chksm=e8df6f6fdfa8e67969540fb98e38dd709b5d3c6ca07bd4a993f70314d86a8691be3029ccdc44&token=866440488&lang=zh_CN#rd)
    - 论文链接：https://arxiv.org/abs/2310.08419
    - 参考链接：https://x.com/llm_sec/status/1718932383959752869?s=20


1. 1Password发布了其安全设计文档，一百多页
    - pdf下载：1passwordstatic.com/files/security/1password-white-paper.pdf ​​​


1. 有3000+ Star的密钥管理项目：Git Secret
    - 常见的一般一些项目的 secrets，都会存储在代码库的外面，防止泄露，使用的时候需要手动去创建，然后去填入，比较麻烦，并且没有 version control，也就不知道添加删除了什么值。#程序员# 
    - Git Secret 可以让这些 secrets 加密的存放在项目中，在使用的时候只需要解密就可以了，这样使用起来很方便。在部署的时候也比原来省心省力了。
    - 地址：github.com/sobolevn/git-secret




















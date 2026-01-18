# Agent Skills：通用 AI 技能库

> 让 AI 快速学会新技能



你好，我是程序员鱼皮。

在前面的文章中，我们学习了如何用 AI 生成代码。但你可能会发现，AI 生成的界面总是千篇一律的蓝紫渐变色，或者在某些特定任务上表现不够专业。

有没有办法让 AI 快速学会新技能，变得更专业呢？

这篇文章，我会介绍 **Agent Skills**，Anthropic 推出的 AI 技能系统，可以让 AI 快速掌握各种专业技能。



## 一、什么是 Agent Skills？

[Agent Skills](https://claude.com/blog/skills) 是 Anthropic 新推出的 AI 技能系统。

它定义了一种 **封装 AI 工作流** 的标准：开发者可以把复杂的任务指令、脚本和资源打包成一个 **技能（Skill）**；作为用户，你只需要安装这些技能，AI 就能立刻学会这项本事，不用重复造轮子。

![](https://pic.yupi.icu/1/%E6%BC%AB%E7%94%BB%E5%9B%BE7%E5%A4%A7.jpeg)



## 二、快速上手 Agent Skills

让我们来实战一下，利用 [frontend-design](https://www.claudeskill.site/en/skills/anthropic-agent-skills:frontend-design) 这个 Agent Skills 来优化生成网站的界面。

### 1、安装 Agent Skills

首先打开 Claude Code，输入一行命令，把官方提供的 Skills 注册为插件市场：

```markdown
/plugin marketplace add anthropics/skills
```

![](https://pic.yupi.icu/1/image-20260116145357194.png)

然后输入 `/plugin`，通过 Tab 键切换到 Marketplaces 界面，批量安装官方提供的 Skills。包括：

- document-skills：文档技能包，可以处理 Excel、Word、PPT、PDF 等文档。
- example-skills：示例技能包 ，可以处理技能创建、构建 MCP、视觉设计、算法艺术、网页测试、动图制作、主题样式等。

![](https://pic.yupi.icu/1/claudecode%E6%8F%92%E4%BB%B6%E5%AE%89%E8%A3%85.png)

安装好之后，输入 `/skills` 命令，就能看到所有已经安装完成的技能了，我们要的 `frontend-design` 也在其中。

![](https://pic.yupi.icu/1/image-20260116145938235.png)

可以在本地找到 Skills 的安装位置，你会发现，SKills 的本质就是一组封装好的提示词文档 + 脚本文件等：

![](https://pic.yupi.icu/1/image-20260116151949110.png)

还有另外一种安装方式，也可以在 Claude Code 中输入一行命令来安装 [frontend-design](https://www.claudeskill.site/en/skills/anthropic-agent-skills:frontend-design) 技能。

```markdown
skill install anthropic-agent-skills:frontend-design
```



### 2、使用 Agent Skills

安装完 SKills 后，你只需要和之前一样跟 AI 对话，程序会自动根据你的任务选择使用什么 Skills。

比如我让 AI 开发一个精美的狼人杀网页游戏，它会询问我是否要使用 `frontend-design` 技能。

![](https://pic.yupi.icu/1/image-20260116152325220.png)

使用这个技能后，AI 会选择独特的设计风格，生成的界面既有个性又专业，告别千篇一律的蓝紫渐变色。而且不需要你每次都重复输入一堆设计要求，非常方便！

![](https://pic.yupi.icu/1/image-20260116153402176.png)

不用技能是这样的，对比一下：

![](https://pic.yupi.icu/1/image-20260116155623890.png)



## 三、更多 Agent Skills

目前 [Anthropic 官方技能仓库](https://github.com/anthropics/skills) 已经提供了丰富的技能集合，涵盖编程相关的数据库优化、API 安全、测试策略、代码审查、文档生成，还有办公相关的 PPT 制作、Excel 处理、Word 文档、PDF 生成等各个方面。

如果官方提供的技能不够用，你还可以上传自定义技能，或者访问 [Claude Skills Hub](https://www.claudeskill.site/) 下载社区贡献的技能。

![](https://pic.yupi.icu/1/image-20260116152552700.png)

值得一提的是，Agent Skills 现已成为 [通用标准](https://agentskills.io)。除了 Claude，[Cursor](https://cursor.com/docs/context/skills) 等主流 AI 编程工具也会陆续提供支持。也就是说，你在一个工具里用的技能，在另一个工具里也能复用。



## 四、Agent Skills 的优势

Agent Skills 最大的优势是 **可复用性**。

以前，如果你想让 AI 生成特定风格的界面，需要每次都写一大段提示词。现在有了 Agent Skills，只需要安装一次技能，以后就能直接使用，不用重复输入。

而且 Agent Skills 是 **跨工具通用** 的。你在 Claude Code 中安装的技能，以后在 Cursor 等其他工具中也能用，不用重复配置。

此外，Agent Skills 是 **社区驱动** 的。任何人都可以创建和分享技能，整个社区的智慧都能为你所用。



## 写在最后

看到这里，相信你已经对 Agent Skills 有了基本的了解。

**Agent Skills 让 AI 能够快速学会新技能，不用每次都重复输入提示词。**

如果你经常需要 AI 完成某些特定的任务，比如生成特定风格的界面、处理特定格式的文档，那么 Agent Skills 会是你的好帮手。

建议你亲自尝试安装几个技能，体验一下 Agent Skills 的便利性。



## 推荐资源

1）鱼皮 AI 导航网站：[AI 资源大全、最新 AI 资讯、免费 AI 教程](https://ai.codefather.cn)

2）编程导航学习圈：[学习路线、编程教程、实战项目、求职宝典、交流答疑](https://www.codefather.cn)

3）程序员面试八股文：[实习/校招/社招高频考点、企业真题解析](https://www.mianshiya.com)

4）程序员写简历神器：[专业模板、丰富例句、直通面试](https://www.laoyujianli.com)

5）1 对 1 模拟面试：[实习/校招/社招面试拿 Offer 必备](https://ai.mianshiya.com)

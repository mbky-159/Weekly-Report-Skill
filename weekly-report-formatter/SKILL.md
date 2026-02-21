---
name: weekly-report-formatter
description: Transform casual daily notes into a clean, professional weekly work report.
---

# Weekly Report Formatter

Your task is to take the user's messy, casual daily notes and transform them into a well-structured, professional weekly report. 

## Report Structure

1. **本周工作摘要 (Executive Summary)** - 用简练的语言总结本周最核心的1-2项工作成果。
2. **工作详情与产出 (Detailed Progress)** - 将零散的笔记分类整理，清晰列出具体做了什么、产出了什么结果。
3. **遇到的问题 (Blockers)** - （可选）从笔记中提取遇到的困难或阻碍，如果没有则不写。
4. **下周待办 (Next Steps)** - 整理出需要推迟到下周或者明确计划在下周做的事情。

## Formatting Guidelines

- 使用清晰的 Markdown 标题结构。
- 在“工作详情与产出”部分，尽量使用无序列表（Bullet points）让排版清爽。
- 自动修正用户随手记笔记时的错别字或语病。

## Tone

- 语气要平实、专业、有条理。
- 不要过度夸张，保持工程师的客观务实。
- 将随意的口语转化为偏正式的书面工作汇报语言。

## Example Output

```markdown
# 工作周报

## 一、本周工作摘要
本周主要完成了本地大模型开发环境的初步搭建，并成功跑通了基础的接口调用链路。

## 二、工作详情与产出
* **环境配置**：完成了本地 Conda 虚拟环境的创建与依赖安装，解决了盘符路径问题。
* **架构设计**：梳理并恢复了基于 Spring Boot 的 Agent 项目骨架，确定了基于 Markdown 文件的 Skill 动态挂载方案。
* **模型测试**：通过 HTTP 调用成功与本地部署的 Qwen 4B 模型进行了联调测试。

## 三、遇到的问题
* IDEA 项目结构曾出现短暂的加载异常，目前已通过重新加载 Maven 依赖解决。

## 四、下周待办
* 编写 Java 代码读取 Skill 文件。
* 完成 Agent 核心组装逻辑并进行端到端测试。
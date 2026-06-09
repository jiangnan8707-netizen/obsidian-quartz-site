# AGENTS.md

这个库是 New Lights 的业务知识中台，用来维护原始资料、业务结论和跨项目事实源。

## 核心模型

- `00-system/` 放规则、模板和提示词。
- `raw/` 里的原始资料是不可变输入。
- `wiki/` 里的页面是基于原始资料整理出来的可编辑总结。
- `index.md` 是业务导航目录。
- `log.md` 是按时间顺序记录的追加日志。

## 工作规则

1. 回答问题时先看 `index.md` 和对应目录页。
2. 原始资料和总结页面要分开。
3. 新证据改变结论时，要更新相关 wiki 页面。
4. 导入、重要提问和检查结果都要记到 `log.md`。
5. 尽量写简短、明确的说明，不要堆大段无结构内容。
6. 发现冲突时要标出来，不要悄悄覆盖。
7. 公司、客户、联系人、产品、市场和长期背景，优先按这个知识库判断。
8. 产品目录册不是完整清单，目录册外的产品也要进知识库。
9. 业务资料优先归类到 `wiki/01-customers/` 到 `wiki/10-company-knowledge/`。

## 推荐流程

- 导入：读一份资料，做摘要，更新目录，更新相关页面，再写日志。
- 查询：先查目录，再读最相关页面，整理答案。如果结果有价值，就留回 wiki。
- 检查：找过时说法、缺失链接、孤立页。
- 日常执行时优先参照 `wiki/overviews/知识库维护规范.md`。
- 跨项目调用和回写时，优先参照 `wiki/overviews/全局调用与回写规则.md`。
- 处理产品资料时，优先参照 `wiki/overviews/产品资料规范.md`。
- 处理业务目录时，优先参照 `wiki/README.md` 和对应的业务目录 README。

## 约定

- 跨页面引用使用 Markdown 链接。
- `index.md` 里写一行摘要。
- `log.md` 只追加，不随便改历史。
- 页面被新版本替代时，要注明替代关系，不要直接抹掉上下文。

## 目录结构

- `00-system/`：规则、模板、提示词。
- `raw/sources/`：不可变的原始资料。
- `raw/assets/`：下载下来的附件和图片。
- `wiki/01-customers/`：客户背调。
- `wiki/02-products/`：产品知识。
- `wiki/03-markets/`：市场分析。
- `wiki/04-competitors/`：竞品与渠道。
- `wiki/05-sales-emails/`：开发信。
- `wiki/06-social-content/`：社媒内容。
- `wiki/07-website-seo/`：网站内容。
- `wiki/08-training/`：业务培训。
- `wiki/09-exhibitions/`：展会资料。
- `wiki/10-company-knowledge/`：公司资料。
- `wiki/overviews/`：高层概览和总览页。
- `wiki/entities/`：实体页。
- `wiki/concepts/`：概念页。
- `wiki/comparisons/`：对比分析页。
- `wiki/notes/`：较小的工作笔记。

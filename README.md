# tech-notes-vault

一个由 [ytkb](https://github.com/yitaohou/ytkb) 自动生成的 Obsidian 技术知识库：把技术类 YouTube 视频拆解成原子概念笔记 + 主题网图 + 完整摘要。

用 Obsidian 直接打开本文件夹即可浏览。

## 结构

- `notes/` — 原子概念笔记，每个概念一个文件，跨视频累积；每条知识点带可点击的 YouTube 时间戳，可跳回原视频对应时刻
- `topics/` — 主题骨架：5 个顶层 topic（ai / frontend / backend / system-design / career-industry）→ subtopic 层，相关 subtopic 互连
- `videos/` — 每个视频一个 hub 笔记（元数据 + 该视频贡献的全部知识点）
- `summaries/` — 每个视频一篇完整摘要（中英混合，概念以 wikilink 链接）
- `topic-map.yaml` — 主题分类的机器可读源

## Graph 视图

过滤栏：`-path:videos -path:summaries` 看纯主题结构；分组着色：`tag:#topic` / `tag:#subtopic` / `tag:#concept` / `tag:#video`。

## 说明

所有笔记均为对原视频内容的改写与整理，附来源链接与时间戳；不包含原始字幕或转录文本。各视频版权归原作者所有，请通过 hub 笔记中的链接观看原视频。

# Personal Portfolio Site Builder

一个帮助新手和设计从业者搭建个人 UI/UX 作品集网站的 Agent Skill。它把个人作品集拆解为可复用的页面结构、项目案例模块和可直接用于提示词的动效名称。

## 包含内容

- `portfolio-site-builder/SKILL.md`：Skill 入口、使用流程和设计原则。
- `portfolio-site-builder/references/page-patterns.md`：首页、项目列表、项目详情、关于和联系页面的结构参考。
- `portfolio-site-builder/references/motion-catalog.md`：动效名称、行为说明、适用场景和实现注意事项。

页面结构与视觉主题分开。当前版本重点是模块搭建和动效；颜色主题预设可在后续版本添加。

## 安装与使用

GitHub 负责托管和分发文件，不会自动把 Skill 加载到每位访客的 Agent。使用者需要将 `portfolio-site-builder` 整个文件夹安装到自己所用 Agent 支持的 Skills 目录，或使用该 Agent 提供的导入功能。

1. 下载或克隆本仓库。
2. 找到仓库中的 `portfolio-site-builder` 文件夹。
3. 将整个文件夹放进 Agent 文档指定的 Skills 目录，或通过 Agent 支持的 Skill 导入功能添加。
4. 在 Agent 中开启新任务，描述要制作的个人作品集网站；可直接说“使用 portfolio-site-builder 帮我搭建作品集网站”。动效可以按词典名称指定，例如“在项目卡片上使用 Staggered Reveal（错峰进入）”。

不同 Agent 的安装位置、发现方式和 Skill 格式支持可能不同。请按所用 Agent 的官方说明安装；不要只复制 `SKILL.md`，否则随附的页面结构和动效参考文件不会一起安装。

## 适用范围

适合规划或实现个人作品集网站、复用页面模块、编排项目案例，以及选择和实现命名动效。Skill 提供的是结构和指导，不会自动提供使用者的个人简介、作品内容、图片或项目成果；使用者需要提供自己的素材。

## 来源与使用边界

本 Skill 的页面和动效模式参考作者自己的作品集源文件整理而成。它提炼可复用的结构和行为，不包含原网站的个人文案、项目素材或源代码。请使用者提供自己的内容，并按自己的需求选择页面结构和视觉风格。

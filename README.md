# Onlyask-skill
By uploading materials and using Socratic questioning to guide your learning, it'll help you explore the entire book, making you fall in love with learning—only by asking questions, you'll gain knowledge spanning ancient times to the present.
# OnlyAsk Skill

> **Only Ask, Never Tell.** 只问不答——用问题引导你自己发现知识的全貌。

一套基于苏格拉底教学法的 AI 辅助自学系统。通过三位可自定义的虚拟老师角色，用问题引导你一步步推理出知识的全貌，同时借助角色扮演和社交互动让学习变得有吸引力。

## 核心特色

- **苏格拉底教学法**：全程用问题引导，不直接给答案，让你自己推理出知识全貌
- **角色沉浸式学习**：三位可自定义的虚拟老师，将学习变成游戏般的体验
- **系统化记忆**：进度追踪、学习日记、群聊互动、角色情感动态演变
- **锚定教材**：教学严格基于你提供的教材，杜绝 AI 幻觉

## 灵感来源

受知乎用户分享的"苏格拉底·三月七"家教系统启发，核心方法论源自苏格拉底教学法（Socratic Method）。

## 适配平台

本 Skill 设计为符合 [TRAE Skill 规范](https://docs.trae.cn/ide_skills.md) 的技能包，可直接安装到 TRAE IDE / TRAE Work 中使用。理论上也可适配 Claude Code、Cursor 等支持项目级指令的 Agentic Coding 工具。

## 安装方法

### 方式一：TRAE IDE / TRAE Work 直接导入

1. 下载本仓库的 zip 压缩包
2. 在 TRAE 中打开 **设置 > 技能与命令**
3. 点击 **创建** > 选择技能类型（全局/项目）
4. 上传 `SKILL.md` 文件或整个仓库的 zip 文件
5. 确认后即可使用

### 方式二：手动放置

1. 将 `onlyask-skill/` 文件夹复制到：
   - **项目级**：`你的项目/.trae/skills/onlyask-skill/`
   - **全局级**：`~/.trae-cn/skills/onlyask-skill/`
2. 确保 `SKILL.md` 在文件夹根目录
3. 重启 TRAE 或刷新技能面板

### 方式三：通过 .agents 目录

1. 将本 Skill 放入项目的 `.agents/skills/onlyask-skill/` 目录
2. 在 TRAE 设置中开启 **启用 .agents 技能目录**

## 使用方法

### 快速开始

安装 Skill 后，在 TRAE 中直接说：

```
我想用苏格拉底教学法学习这本教材 [教材文件路径]
```

AI 会自动初始化系统，询问你的个人信息和角色偏好。

### 自定义角色

你可以设定任何角色作为虚拟老师：
- 二次元角色（如崩铁的三月七、甘雨、刻晴等）
- 历史人物（如图灵、爱因斯坦、孔子等）
- 明星、学者、作家等
- 甚至小动物

每位角色有独立的性格、教学风格和互动方式。

### 日常流程

1. **上课**：告诉 AI 想学哪一章、由哪位角色授课
2. **课中**：自由提问、查看群聊（"我想看看群聊"）、换角色
3. **下课**：说"下课了"，AI 自动更新所有记录
4. **下次**：新对话自动恢复上次进度

## 文件结构

### Skill 包（本仓库）

```
onlyask-skill/
├── SKILL.md                          # 技能核心定义（TRAE Skill 规范）
├── README.md                         # 本文件
├── LICENSE                           # MIT 开源协议
├── resources/
│   ├── system_full.md                # 系统完整规则参考
│   ├── character_template.md         # 角色人设模板
│   └── revision_format.md            # 教材改进记录格式
├── templates/
│   └── system_template.md           # 系统初始化模板
└── examples/
    └── usage_example.md             # 使用示例
```

### 初始化后在项目中生成

```
onlyask-teacher/
├── system.md              # 系统文档
├── system_detail.md       # 补充设定（故事背景）
├── progress.md            # 学习进度
├── learner_profile.md     # 学习者档案
├── character_a.md         # 角色 A 人设
├── character_b.md         # 角色 B 人设
├── character_c.md         # 角色 C 人设
├── group_chat.md          # 群聊记录
├── chat_unread.md         # 未读消息
├── diary.md              # 学习日记
├── book_revision_notes.md # 教材改进笔记
├── session_archive.md    # 历史存档
└── tmp/                  # 临时文件（公式渲染）
```

## 教学原理

### 苏格拉底式提问六层次

1. **澄清性**：你是怎么理解的？
2. **探究假设**：这个前提成立吗？
3. **探索证据**：有什么证据支持？
4. **替代观点**：有没有其他解释？
5. **推导后果**：成立的话会带来什么影响？
6. **元认知反思**：我们是怎么得到这个结论的？

### 为什么有效

- 主动思考 > 被动接受
- 自我推理的记忆深刻度远高于被告知答案
- 角色扮演提供情感激励，解决学习动力问题
- 系统化记忆实现长期持续学习

## 许可证

MIT License - 自由使用、修改和分发。

## 致谢

- 灵感来自知乎"苏格拉底·三月七"家教系统的分享
- 苏格拉底教学法（Socratic Method）
- [TRAE Skill 规范](https://docs.trae.cn/ide_skills.md)

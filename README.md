# AI Agent Skills Start

个人 AI Agent Skill 项目集合，包含自定义 WorkBuddy Skill 及配套工具链。

## 项目结构

```
.
├── ai-dev-pipeline.zip   # ai-dev-pipeline Skill 打包文件
├── .workbuddy/           # WorkBuddy 工作数据
│   ├── memory/            # 跨会话记忆存储
│   └── skills/           # 用户级 Skill 存放目录
└── README.md
```

## Skills 说明

### ai-dev-pipeline

AI 项目全流程开发助手，覆盖从需求分析到自动化编码的完整流程。

**触发词：**
- 「帮我开发一个项目」
- 「开始新项目」
- 「从头做一个 xxx」
- 「项目开发流程」

**流程阶段：**
1. **需求分析** — 主动提问，生成 `docs/proposal.md`
2. **系统设计** — 模块化架构设计，生成 `docs/design.md`
3. **任务拆解** — 生成 Checklist 任务清单 `progress.md` + `docs/tasks/`
4. **自动化编码指挥** — 生成 `prompt.md`，指导 AI 按模块顺序自动开发

**特点：**
- 每次执行前询问项目目录，支持自定义项目代码文件夹名称
- 支持上传 UI 风格文件，约束后续所有阶段的输出风格
- 测试/检查工具按技术栈自适应（PHP/Python/Node.js/Java/Go）
- 输出 `prompt.md` 后引导用户复制到新对话执行自动开发

## 安装方法

1. 打开 WorkBuddy
2. 进入「专家」→「Skill 管理」
3. 上传 `ai-dev-pipeline.zip`
4. 安装完成后即可通过触发词使用

## 环境要求

- WorkBuddy 平台
- 支持 Windows / macOS / Linux

##  License

MIT

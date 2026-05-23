# AI Agent Skills Start

个人 AI Agent Skill 项目集合，包含自定义 WorkBuddy Skill 及配套工具链。

## 项目结构

```
.
├── ai-dev-pipeline/      # ai-dev-pipeline Skill 源文件
│   └── SKILL.md
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

**方式一：从源文件安装（推荐）**
1. 克隆本仓库到本地
2. 将 `ai-dev-pipeline/` 文件夹复制到 WorkBuddy 用户 Skill 目录：
   - Windows：`C:/Users/你的用户名/.workbuddy/skills/`
   - macOS/Linux：`~/.workbuddy/skills/`
3. 重启 WorkBuddy，Skill 自动生效

**方式二：打包安装**
1. 使用 WorkBuddy 的 Skill 管理工具将 `ai-dev-pipeline/` 打包为 `.zip`
2. 打开 WorkBuddy → 「专家」→「Skill 管理」
3. 上传打包后的 `.zip` 文件
4. 安装完成后即可通过触发词使用

## 环境要求

- WorkBuddy 平台
- 支持 Windows / macOS / Linux

## License

MIT

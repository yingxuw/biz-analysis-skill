# Biz Analysis Skill — 发布物料

## 📦 发布清单

- [x] SKILL.md（核心技能文档）
- [x] README.md（项目说明）
- [x] TEMPLATE.md（快速应用模板）
- [x] CHECKLIST.md（输出核验清单）
- [x] EXAMPLES.md（成功案例参考）
- [ ] LICENSE（许可证）
- [ ] .gitignore
- [ ] 发布说明（RELEASE.md）

---

## 🚀 GitHub 发布步骤

### 1. 创建仓库

**方式A：GitHub 网页版**
1. 访问 https://github.com/new
2. 仓库名：`biz-analysis-skill`
3. 描述：`深度业务分析框架 — 产出有数据支撑、有竞品对标、有可执行优先级的分析报告`
4. 选择：Public（或 Private）
5. 点击「Create repository」

**方式B：GitHub CLI**
```bash
gh repo create biz-analysis-skill \
  --public \
  --description "深度业务分析框架" \
  --homepage "https://github.com/your-org/biz-analysis-skill"
```

---

### 2. 上传文件

**方式A：Git 命令行**
```bash
cd /Users/tal/Documents/Obsidian\ Vault/.claude/skills/biz-analysis/github-release

git init
git add .
git commit -m "feat: 发布 Biz Analysis Skill v1.0"
git branch -M main
git remote add origin https://github.com/<your-username>/biz-analysis-skill.git
git push -u origin main
```

**方式B：GitHub 网页版**
1. 进入仓库页面
2. 点击「Add file」→「Upload files」
3. 拖拽 `github-release/` 目录下所有文件
4. Commit 消息：`feat: 发布 Biz Analysis Skill v1.0`
5. 点击「Commit changes」

---

### 3. 创建 Release

**方式A：GitHub 网页版**
1. 进入仓库 →「Releases」→「Create a new release」
2. Tag version：`v1.0.0`
3. Release title：`Biz Analysis Skill v1.0.0 — 深度业务分析框架`
4. Description：

```markdown
## 🎉 首次发布

这是 **Biz Analysis Skill** 的第一个正式版本，一套经过验证的业务分析框架。

### ✨ 核心特性

- ✅ **五步分析法**：收集输入 → 构建Prompt → 标准分析 → 迭代循环 → 输出核验
- ✅ **结构化输出**：全景梳理、效果对比、规律提炼、竞品对标、用户分层、优先级
- ✅ **可执行清单**：每项建议包含预期效果 + 数据支撑 + 成本估计
- ✅ **迭代机制**：内置质疑清单，确保结论经得起推敲

### 📦 物料

- `SKILL.md` — 核心技能文档（完整框架）
- `TEMPLATE.md` — 快速应用模板（直接套用）
- `CHECKLIST.md` — 输出核验清单（5步核验法）
- `EXAMPLES.md` — 成功案例参考（天天练活动策略分析）

### 🚀 快速开始

```markdown
@.claude/skills/biz-analysis/SKILL.md 帮我分析 [业务名称] 的 [核心问题]
```

详细使用说明见 [README.md](https://github.com/your-org/biz-analysis-skill/blob/main/README.md)

### 📝 使用场景

- 商业化活动分析
- 用户增长分析
- 产品功能评估
- 运营策略复盘
- 新业务调研

### 🤝 贡献

欢迎提交 Issue 和 PR！

### 📄 License

MIT
```

5. 点击「Publish release」

**方式B：GitHub CLI**
```bash
gh release create v1.0.0 \
  --title "Biz Analysis Skill v1.0.0 — 深度业务分析框架" \
  --notes-file RELEASE.md \
  --latest
```

---

### 4. 生成下载链接

Release 发布后，会生成如下文件下载链接：

```
https://github.com/<your-username>/biz-analysis-skill/releases/download/v1.0.0/SKILL.md
https://github.com/<your-username>/biz-analysis-skill/releases/download/v1.0.0/TEMPLATE.md
https://github.com/<your-username>/biz-analysis-skill/releases/download/v1.0.0/CHECKLIST.md
https://github.com/<your-username>/biz-analysis-skill/releases/download/v1.0.0/EXAMPLES.md
```

**用户可以通过这些链接直接下载单个文件**，无需克隆整个仓库。

---

## 📋 发布说明（RELEASE.md）

```markdown
# Biz Analysis Skill v1.0.0

## 🎯 新增功能

- **五步分析法**：收集输入 → 构建Prompt → 标准分析 → 迭代循环 → 输出核验
- **结构化输出框架**：6个必选模块（全景梳理、效果对比、规律提炼、竞品对标、用户分层、优先级）
- **迭代循环机制**：内置质疑清单，确保结论经得起推敲
- **输出核验清单**：5步核验法，避免常见错误

## 📦 物料包

- `SKILL.md` — 核心技能文档（185行）
- `TEMPLATE.md` — 快速应用模板
- `CHECKLIST.md` — 输出核验清单
- `EXAMPLES.md` — 成功案例参考

## 🚀 快速开始

1. 复制 SKILL.md 到 Obsidian vault 的 `.claude/skills/biz-analysis/` 目录
2. 在笔记中调用：`@.claude/skills/biz-analysis/SKILL.md 帮我分析 XX 业务`
3. 按 TEMPLATE.md 提供背景、目标、约束信息

## 📖 文档

- [完整使用指南](https://github.com/your-org/biz-analysis-skill/blob/main/README.md)
- [成功案例](https://github.com/your-org/biz-analysis-skill/blob/main/EXAMPLES.md)

## 🤝 贡献

欢迎提 Issue 和 PR！

## 📄 License

MIT
```

---

## 🎨 宣传物料（让别人能通过链接下载）

### 1. README 摘要（可复制到朋友圈/社群）

```
📊 Biz Analysis Skill — 深度业务分析框架

一套结构化、可复用的业务分析 Skill，产出有数据支撑、有竞品对标、有可执行优先级的分析报告。

✅ 五步分析法
✅ 6个必选模块
✅ 内置质疑清单
✅ 可执行优先级清单

🚀 快速使用：
@.claude/skills/biz-analysis/SKILL.md 帮我分析 [业务] 的 [问题]

📦 下载：https://github.com/your-org/biz-analysis-skill/releases/latest
```

### 2. 使用指南卡片

```
┌─────────────────────────────────────┐
│  Biz Analysis Skill                 │
├─────────────────────────────────────┤
│  适用场景：                          │
│  • 商业化活动分析                   │
│  • 用户增长分析                     │
│  • 产品功能评估                     │
│  • 运营策略复盘                     │
│  • 新业务调研                       │
├─────────────────────────────────────┤
│  快速开始：                          │
│  1. 下载 SKILL.md                   │
│  2. 放到 .claude/skills/ 目录       │
│  3. 调用：@SKILL.md 分析XX业务       │
├─────────────────────────────────────┤
│  下载链接：                          │
│  github.com/xxx/biz-analysis-skill  │
└─────────────────────────────────────┘
```

---

## 📤 分享方式

### 方式1：直接分享 Release 页面

```
https://github.com/<your-username>/biz-analysis-skill/releases/latest
```

用户点击即可下载所有文件。

### 方式2：分享单个文件链接

```
https://github.com/<your-username>/biz-analysis-skill/releases/download/v1.0.0/SKILL.md
```

### 方式3：生成二维码

用上述链接生成二维码，方便扫码下载。

---

## 🔧 后续维护

### 版本规划

- v1.1.0：增加更多行业案例（游戏/电商/教育）
- v1.2.0：提供 Python 脚本自动化分析
- v2.0.0：支持多语言（英文版）

### 收集反馈

- 在 GitHub 开 Issue 收集使用反馈
- 定期更新成功案例（EXAMPLES.md）
- 迭代 CHECKLIST（优化核验点）

---

**准备好了吗？** 按步骤执行即可完成发布。

**需要我帮你生成完整的 RELEASE.md 文件吗？**

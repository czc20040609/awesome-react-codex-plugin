# Awesome React Codex Plugin

## 中文

这是一个用于 Codex 的 React / React Native 前端开发 skill。它适合在每次编写前端代码时使用，覆盖功能开发、组件设计、组件库选型、调试、重构、代码审查、测试和学习解释。

插件内置 [enaqx/awesome-react](https://github.com/enaqx/awesome-react) 资源目录，可用于查找 React 框架、组件库、状态管理、表单、路由、测试、图表、地图、动画和 React Native 工具。资源目录是快照，正式采用前请核对官方文档、版本、兼容性、维护状态和许可证。

### 三个平台一键安装

前置条件：已安装 Git 和 Codex CLI。

#### macOS（zsh）

```bash
git clone https://github.com/czc20040609/awesome-react-codex-plugin.git "$HOME/.codex/awesome-react-codex-plugin" && \
codex plugin marketplace add "$HOME/.codex/awesome-react-codex-plugin" && \
codex plugin add awesome-react@awesome-react-codex-plugin
```

#### Linux（bash）

```bash
git clone https://github.com/czc20040609/awesome-react-codex-plugin.git "$HOME/.local/share/awesome-react-codex-plugin" && \
codex plugin marketplace add "$HOME/.local/share/awesome-react-codex-plugin" && \
codex plugin add awesome-react@awesome-react-codex-plugin
```

#### Windows（PowerShell）

```powershell
$pluginRoot = Join-Path $env:LOCALAPPDATA "Codex\awesome-react-codex-plugin"
git clone https://github.com/czc20040609/awesome-react-codex-plugin.git $pluginRoot
if ($LASTEXITCODE -eq 0) { codex plugin marketplace add $pluginRoot }
if ($LASTEXITCODE -eq 0) { codex plugin add awesome-react@awesome-react-codex-plugin }
```

安装后请新开一个 Codex 任务，让 skill 生效。

## English

This is a Codex skill for React and React Native frontend development. Use it whenever you write frontend code: feature implementation, component design, component-library selection, debugging, refactoring, code review, testing, and learning.

It includes a snapshot of [enaqx/awesome-react](https://github.com/enaqx/awesome-react) for discovering React frameworks, component libraries, state management, forms, routing, testing, charts, maps, animation, and React Native tools. The catalog is a discovery index; verify current documentation, versions, compatibility, maintenance status, and licensing before adopting a dependency.

### One-command installation on three systems

Prerequisites: Git and the Codex CLI.

#### macOS (zsh)

```bash
git clone https://github.com/czc20040609/awesome-react-codex-plugin.git "$HOME/.codex/awesome-react-codex-plugin" && \
codex plugin marketplace add "$HOME/.codex/awesome-react-codex-plugin" && \
codex plugin add awesome-react@awesome-react-codex-plugin
```

#### Linux (bash)

```bash
git clone https://github.com/czc20040609/awesome-react-codex-plugin.git "$HOME/.local/share/awesome-react-codex-plugin" && \
codex plugin marketplace add "$HOME/.local/share/awesome-react-codex-plugin" && \
codex plugin add awesome-react@awesome-react-codex-plugin
```

#### Windows (PowerShell)

```powershell
$pluginRoot = Join-Path $env:LOCALAPPDATA "Codex\awesome-react-codex-plugin"
git clone https://github.com/czc20040609/awesome-react-codex-plugin.git $pluginRoot
if ($LASTEXITCODE -eq 0) { codex plugin marketplace add $pluginRoot }
if ($LASTEXITCODE -eq 0) { codex plugin add awesome-react@awesome-react-codex-plugin }
```

Start a new Codex task after installation so the skill is loaded.

Source snapshot: commit `e6fd973eefe57d288a60e6d21bb9d8f343addfe9`.

## License

Original plugin material is licensed under MIT. The bundled `awesome-react.md` catalog is excluded from that license and remains under its upstream CC BY 4.0 terms; see the repository's [THIRD_PARTY_NOTICES.md](../../THIRD_PARTY_NOTICES.md).

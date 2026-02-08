<div align="center">

<br/>

<img src="https://grovetools.ai/docs/grove/images/grove-logo-with-text-dark.svg" alt="Grove" width="180">

<br/>
<br/>

### Local-first, terminal-based toolkit for AI-assisted software development

<br/>

<a href="https://grovetools.ai">
  <img src="https://img.shields.io/badge/Documentation-grovetools.ai-8A2BE2?style=for-the-badge" alt="Documentation">
</a>

<br/>
<br/>

---

</div>

<br/>

Grove aims to make coding with AI feel more deliberate, controlled, and organized. It primarily serves as an orchestration layer for agents like Claude Code and LLM API calls. Grove also has tools for context engineering, information management, workspace discovery, project navigation, and scenario-based testing. It integrates with tmux and Neovim.

<br/>

### Context Engineering

Context engineering is critical for making AI coding feel controlled and accurate. Grove uses `cx` rules files to define context with `.gitignore`-style patterns. These can pull in code from across the filesystem or from GitHub by commit, ref, or tag. Rules files can be saved, pinned to jobs, and imported by other repositories. Running `cx generate` produces context bundles that can be uploaded to LLM APIs along with prompts, producing better plans in a fraction of the time compared to an agent's Plan Mode.

### Markdown Orchestration

Grove's approach to orchestration is Markdown-based. Workflows are defined as Plans, directories of Markdown files where each file represents a Job. Jobs define dependencies, creating a DAG of tasks. They can contain rough ideas, bug reports, or complete specifications. They can be submitted to LLM APIs to create one-shot plans, or serve as briefings for coding agents. Grove keeps everything as plain text so it remains accessible to both agents and humans.

### Workspaces

AI-assisted coding enables exploring many ideas as new projects or features. Grove's Workspace Model manages this complexity. Create new repositories or worktrees instantly, then clean them up when done. Jump to any project or worktree with a few keystrokes. Know where agents are running or idle, and hop between them. Grove can instantiate synchronized worktrees across multiple repositories, allowing agents to make changes across microservices or libraries in a single, isolated directory.

### Notebooks

Each repository is paired with a sister notebook directory elsewhere on the filesystem. Notebooks store ideas, issues, plans, jobs, todos, project concepts, agent skills, and draft documentation. Notes can be promoted to `flow` plans, creating new worktrees in which to develop. Notebooks persist across branches and worktrees, offering knowledge management that is stored separately from the code.

<br/>

---

<div align="center">

<br/>

### Tools

<br/>

| | |
|:--|:--|
| [**cx**](https://github.com/grovetools/cx) | Context bundles from glob rules with token analysis |
| [**flow**](https://github.com/grovetools/flow) | Markdown orchestration for plans and agent lifecycles |
| [**nav**](https://github.com/grovetools/nav) | Keyboard-focused tmux session manager |
| [**nb**](https://github.com/grovetools/nb) | Workspace-aware notebook manager |
| [**hooks**](https://github.com/grovetools/hooks) | Agent observability and state tracking |
| [**grove.nvim**](https://github.com/grovetools/grove.nvim) | Neovim plugin for context and plans |
| [**grove**](https://github.com/grovetools/grove) | Meta-CLI and package manager |
| [**tend**](https://github.com/grovetools/tend) | Scenario-based E2E testing |
| [**docgen**](https://github.com/grovetools/docgen) | LLM-powered documentation generator |
| [**skills**](https://github.com/grovetools/skills) | Agent skill management |

<br/>

</div>

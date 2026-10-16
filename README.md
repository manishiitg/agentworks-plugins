# AgentWorks plugins

Plugins that connect Claude Code, Codex, Muse, Pi and Cursor chats to
[AgentWorks](https://github.com/manishiitg/agentworks) (AgentBridge messaging).
This repository is generated from `plugins/` and the marketplace manifests in
the main repository on every change; send fixes there, not here.

```sh
claude plugin marketplace add manishiitg/agentworks-plugins
claude plugin install agentworks@agentworks

codex plugin marketplace add manishiitg/agentworks-plugins
codex plugin add agentworks-codex@agentworks

muse plugins marketplace add agentworks https://github.com/manishiitg/agentworks-plugins.git
muse plugins install agentworks-muse@agentworks

cursor-agent plugin marketplace add https://github.com/manishiitg/agentworks-plugins.git
```

Cursor CLI also supports loading `plugins/cursor` with `--plugin-dir`. Review
its [project-hook setup and tested modes](plugins/cursor/README.md) before
attaching; desktop messaging has separate limitations.

Already installed from the main repository? It keeps working. To switch to this
smaller source, remove the old marketplace and add this one (see each plugin's
README).

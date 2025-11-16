# Tâches CC Prompts

A collection of Claude Code slash command prompts for enhanced workflow management.

## Overview

This repository contains reusable slash command prompts for Claude Code that enhance productivity through:

- **Meta-prompting**: Self-improving prompt patterns
- **Todo management**: Task tracking and organization
- **Context handoff**: Maintaining context across sessions

## Installation

```bash
# Clone the repo
git clone https://github.com/zerog-arlekin/taches-cc-prompts.git
cd taches-cc-prompts

# Install meta-prompting commands
cp meta-prompting/*.md ~/.claude/commands/

# Install todo management commands
cp todo-management/*.md ~/.claude/commands/

# Install context handoff commands
cp context-handoff/*.md ~/.claude/commands/
```

## Directory Structure

```
taches-cc-prompts/
├── meta-prompting/       # Self-improving prompt patterns
├── todo-management/      # Task tracking commands
├── context-handoff/      # Context preservation across sessions
└── README.md
```

## Usage

After installation, use the slash commands in Claude Code:

```
/meta-analyze          # Analyze and improve prompts
/todo-init             # Initialize task tracking
/context-save          # Save current context
/context-restore       # Restore previous context
```

## Contributing

Contributions welcome! Please submit pull requests with new prompt patterns.

## License

MIT

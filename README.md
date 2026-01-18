# crypteras-orchestrator

Orquestrador de IA do crypteras

## 📚 Documentation

This orchestrator manages the Context-First development methodology for the project.

## 🏗️ Structure

```
crypteras-orchestrator/
├── .claude/
│   └── commands/            # Command definitions for AI
│       ├── products/        # Product commands (collect, refine, spec, check)
│       ├── engineer/        # Engineering commands (start, plan, work, pre-pr, pr)
│       ├── quality/         # Quality commands (observe, metrics)
│       └── warm-up.md       # Context loading command
├── .sessions/               # Feature session data (gitignored)
├── ai.properties.md         # Configuration (gitignored - each dev has their own)
└── context-manifest.json    # Repository manifest
```

## ⚙️ Configuration

Edit `ai.properties.md` to configure:
- Project paths (specific to each developer)
- Task manager credentials (linear)
- Branch conventions
- Repository-specific commands

**Note**: `ai.properties.md` is gitignored because it contains local paths and credentials specific to each developer.

## 🚀 Usage

1. Configure `ai.properties.md` with your project paths
2. Define your repositories in `context-manifest.json`
3. Use `context-cli` to manage features and workspaces

## 📝 License

MIT

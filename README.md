# BMAD-ph.d

A powerful AI-assisted development framework featuring the Business-Minded Application Development (BMAD) core system with specialized extensions.

## 🚀 Latest Addition: Ph.D. Paper Writing Team

We've added a comprehensive academic paper writing system to BMAD! The Ph.D. Paper Writing Team helps researchers write high-quality papers for data science conferences.

## Documentation

- [Ph.D. Paper Writing Team Guide](docs/README-paper-team.md)
- [Architecture Document](docs/architecture.md)
- [BMAD Core User Guide](.bmad-core/user-guide.md)

### Key Features

- **4 Specialized Ph.D. Agents**: Researcher, Paper Expert, Reviewer, and Writer
- **Team-Level Commands**: Including the new `*start-paper` command for streamlined workflow
- **Conference-Ready Templates**: Support for NeurIPS, ICML, KDD, and more
- **Quality Assurance**: Built-in peer review simulation and checklists
- **Collaborative Integration**: Works with existing BMAD agents (Analyst, Architect, Dev)

### Quick Start

```bash
# Activate the paper writing team
*activate team-paper-writing

# Start a new paper project (recommended)
*start-paper

# Or use quick start
*start-paper quick "Your Research Topic" NeurIPS 2024-06-01

# Check progress anytime
*status
```

📚 **Full Documentation**: See [Ph.D. Paper Writing Team Guide](docs/README-paper-team.md)

## Installation

1. Clone this repository
2. Navigate to the project directory
3. Activate your desired team:
   ```bash
   @{team}.md
   *activate team-{team-name}
   ```

## Project Structure

```
BMAD-ph.d/
├── bmad-core/           # Core BMAD framework
│   ├── agents/          # Individual agent definitions
│   ├── agent-teams/     # Team configurations
│   ├── tasks/           # Executable task workflows
│   ├── templates/       # Document templates
│   ├── checklists/      # Quality checklists
│   └── workflows/       # End-to-end workflows
├── docs/                # Documentation
│   ├── README-paper-team.md  # Paper team guide
│   └── architecture.md       # System architecture
└── papers/              # Paper projects workspace
```

## Usage Examples

```bash
# Interactive mode (recommended)
*activate team-paper-writing
*start-paper

# Quick start mode
*activate team-paper-writing
*start-paper quick "ML Fairness Research" NeurIPS 2024-06-01

# Check progress
*status
```

## Contributing

To extend these team:

1. Add new agents in `.bmad-core/agents/`
2. Create tasks in `.bmad-core/tasks/`
3. Define workflows in `.bmad-core/workflows/`
4. Configure teams in `.bmad-core/agent-teams/`

## License

This project is part of the BMAD framework ecosystem.

---

For questions or support, activate any agent and ask for help!

# Ph.D. Paper Writing Team - User Guide

## Overview

The Ph.D. Paper Writing Team is an extension of the BMAD framework designed to help researchers write high-quality academic papers for data science conferences. This team consists of four specialized AI agents who collaborate to guide you through the entire paper writing process.

## Team Members

### 🔬 Prof. Kown - Research Strategy & Ideation Expert

- **Role**: Lead researcher who generates novel research questions
- **Expertise**: Literature analysis, hypothesis generation, experimental design
- **When to use**: Starting a new research project, finding research gaps, designing experiments

### 📐 Dr. Marcus - Academic Paper Structure Architect

- **Role**: Designs optimal paper structure for specific conferences
- **Expertise**: Conference requirements, narrative flow, space optimization
- **When to use**: Planning paper structure, organizing content, meeting page limits

### 🔍 Dr. Elena - Academic Content Quality Assurance

- **Role**: Ensures research quality and academic standards
- **Expertise**: Methodology validation, peer review, academic writing standards
- **When to use**: Reviewing drafts, checking technical accuracy, preparing for submission

### ✍️ Dr. James - Academic Writing Specialist

- **Role**: Creates clear, engaging academic prose
- **Expertise**: Technical writing, citation management, clarity optimization
- **When to use**: Writing sections, improving clarity, polishing prose

## Getting Started

### 1. Activate the Team

```bash
*activate team-paper-writing
```

### 2. Start a New Paper Project

```bash
*start-paper
```

This team-level command will guide you through:

- Setting up paper metadata (title, conference, deadline)
- Creating project workspace structure
- Selecting appropriate workflow (full paper, quick review, or survey)
- Automatically activating the first agent (Dr. Kwon for research)
- Beginning the ideation phase

For quick setup with defaults:

```bash
*start-paper quick "Your Research Topic" NeurIPS 2024-06-01
```

### 3. Team-Level Commands

These commands work across all agents:

- `*help` - Show all team and agent commands
- `*start-paper` - Begin new paper project with guided setup
- `*status` - Show current paper project status and progress
- `*team-status` - Display active agents and their tasks
- `*switch-workflow` - Change workflow type
- `*paper-dashboard` - Overview of all paper projects

### 4. Individual Agent Commands

#### Researcher Commands

- `*ideate {topic}` - Generate research ideas
- `*analyze-gaps {field}` - Find literature gaps
- `*design-experiment` - Design experimental framework

#### Paper Expert Commands

- `*structure {conference}` - Create paper structure
- `*optimize-flow` - Improve narrative flow
- `*format-check` - Verify conference compliance

#### Reviewer Commands

- `*review {section}` - Review specific section
- `*validate-methodology` - Check research methods
- `*execute-checklist` - Run quality checklists

#### Writer Commands

- `*write {section}` - Write paper section
- `*enhance-clarity` - Improve readability
- `*write-abstract` - Create paper abstract

## Workflow Overview

The team follows a structured workflow with five main phases:

### Phase 1: Research Ideation (2-3 days)

- Explore research topics
- Identify gaps in literature
- Assess feasibility
- Define research questions

### Phase 2: Paper Structure Design (1 day)

- Analyze conference requirements
- Design section layout
- Allocate space efficiently
- Plan narrative arc

### Phase 3: Content Creation (5-10 days)

- Write each section iteratively
- Collaborate between agents
- Integrate feedback continuously
- Maintain technical accuracy

### Phase 4: Review and Refinement (3-5 days)

- Technical accuracy review
- Clarity and flow optimization
- Methodology validation
- Iterative improvements

### Phase 5: Final Polish (1-2 days)

- Format verification
- Final quality checks
- Submission preparation
- Conference compliance

## Customizing for Your Research Domain

### Modifying Agent Personas

Each agent's behavior can be customized by editing their persona file in `bmad-core/agents/`. Key areas to customize:

1. **Core Principles**: Add domain-specific principles
2. **Commands**: Add specialized commands for your field
3. **Dependencies**: Link to custom templates or checklists

Example customization for bioinformatics:

```yaml
persona:
  core_principles:
    - Biological relevance validation
    - Statistical rigor for genomic data
    - Reproducible computational pipelines
```

### Creating Custom Templates

Templates are in `bmad-core/templates/`. To create a conference-specific template:

1. Copy `conference-paper-tmpl.yaml`
2. Rename for your conference
3. Modify sections and requirements
4. Update page limits and formatting

### Adding Domain-Specific Checklists

Create new checklists in `bmad-core/checklists/` for your research area:

- Method-specific validation
- Domain ethical considerations
- Field-specific reproducibility

## Integration with Existing BMAD Agents

The paper writing team seamlessly integrates with existing BMAD agents:

### Analyst ↔ Researcher

- **Use case**: Data-driven research insights
- **Example**: `*collaborate-analyst` during ideation
- **Benefit**: Grounds research in data analysis

### Architect ↔ Paper Expert

- **Use case**: System design papers
- **Example**: Structure system architecture sections
- **Benefit**: Technical depth in system descriptions

### Dev ↔ Writer

- **Use case**: Implementation details
- **Example**: Writing method implementation sections
- **Benefit**: Accurate technical descriptions

## Best Practices

### 1. Start Early

- Begin ideation well before conference deadlines
- Allow time for multiple revision cycles
- Plan for unexpected research challenges

### 2. Iterate Frequently

- Get feedback after each section
- Don't wait until the end to review
- Make incremental improvements

### 3. Use All Team Members

- Each agent has unique expertise
- Collaborate between agents
- Don't skip the review phase

### 4. Customize for Your Conference

- Check specific requirements early
- Adapt templates to conference style
- Verify all special sections included

### 5. Maintain Version Control

- Save drafts after each phase
- Track changes and feedback
- Keep experimental versions

## Common Scenarios

### Scenario 1: Starting from Scratch (Recommended)

```bash
*activate team-paper-writing
*start-paper
# Follow guided setup for conference, deadline, topic
# Automatically begins with Dr. Kwon for ideation
```

Or for quick start:

```bash
*activate team-paper-writing
*start-paper quick "fairness in machine learning" NeurIPS 2024-06-01
```

### Scenario 2: Improving Existing Draft

```bash
*activate reviewer
*review introduction
*activate writer
*enhance-clarity
```

### Scenario 3: Conference Adaptation

```bash
*activate paper-expert
*format-check "ICML"
*optimize-flow
```

### Scenario 4: Check Progress

```bash
*status  # Shows current paper progress and timeline
*team-status  # Shows which agents are active
*paper-dashboard  # Overview of all papers
```

## Troubleshooting

### Paper Exceeds Page Limit

1. Run `*optimize-flow` with paper expert
2. Identify content for supplementary material
3. Use `*enhance-clarity` to tighten prose

### Weak Research Motivation

1. Return to researcher agent
2. Run `*analyze-gaps` for better positioning
3. Strengthen introduction with findings

### Poor Review Feedback

1. Use reviewer agent's detailed checklists
2. Address each concern systematically
3. Validate changes with `*review`

## Advanced Features

### Custom Workflows

Create specialized workflows in `bmad-core/workflows/`:

- Workshop paper workflow
- Journal extension workflow
- Fast-track submission workflow

### Multi-Paper Management

- Use paper IDs to track multiple projects
- Switch contexts between papers
- Maintain separate workspaces

### Conference-Specific Optimization

- Load conference-specific templates
- Apply formatting automatically
- Check requirements dynamically

## Tips for Success

1. **Trust the Process**: Follow the workflow phases
2. **Be Specific**: Provide detailed context to agents
3. **Iterate**: First drafts are never perfect
4. **Collaborate**: Use agent interactions
5. **Stay Organized**: Use the file structure

## Getting Help

- Run `*help` with any agent for commands
- Check templates for section guidance
- Review checklists before submission
- Examine example papers in your field

## Contributing

To improve the paper writing team:

1. Share successful templates
2. Add conference requirements
3. Contribute domain-specific checklists
4. Report workflow improvements

---

Remember: The Ph.D. Paper Writing Team is here to guide and support your research communication. While the agents provide structure and expertise, your unique research insights and domain knowledge are what make great papers. Use this team as a collaborative partner in your academic journey!

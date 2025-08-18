# Paper Status Task

## Task Overview

This task displays the current status of active paper projects, showing progress through workflow phases and upcoming deadlines.

## Activation

When user runs `*status` command at team or agent level.

## Process

### Check Active Projects

1. **Scan for Active Papers**

   - Look in papers/ directory
   - Find projects with status != 'completed'
   - Load metadata for each

2. **Determine Current Project**
   - If only one active: show that
   - If multiple: list and ask which
   - If none: suggest \*start-paper

### Display Status Dashboard

```
📊 Paper Status Dashboard
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Paper: {{title}}
ID: {{paper-id}}
Conference: {{conference}} | Deadline: {{deadline}} ({{days_remaining}} days)

Current Phase: {{phase_name}} ({{phase_progress}}%)
├── Started: {{phase_start_date}}
├── Duration: {{elapsed_days}}/{{estimated_days}} days
└── Status: {{on_track|delayed|ahead}}

Active Agent: {{agent_name}}
Current Task: {{task_name}}

Progress Overview:
✅ Research Ideation     [████████████] 100% | 2 days
🔄 Structure Design      [████░░░░░░░░] 35%  | 0.5 days
⏳ Content Creation      [░░░░░░░░░░░░] 0%   | Pending
⏳ Review & Refinement   [░░░░░░░░░░░░] 0%   | Pending
⏳ Final Polish          [░░░░░░░░░░░░] 0%   | Pending

Recent Activity:
- {{timestamp}}: Research questions finalized
- {{timestamp}}: Started paper structure design
- {{timestamp}}: Conference requirements loaded

Next Milestones:
□ Complete paper structure ({{target_date}})
□ First draft introduction ({{target_date}})
□ Complete method section ({{target_date}})

Quick Actions:
1. Continue with current task
2. Switch to different agent
3. View detailed progress
4. Adjust timeline
5. Export status report

Select action or press Enter to continue:
```

### Phase-Specific Details

#### If in Ideation Phase:

```
Research Progress:
- Research Questions: {{count}} generated
- Feasibility: {{assessed|pending}}
- Literature Gaps: {{identified|in-progress}}
```

#### If in Structure Phase:

```
Structure Progress:
- Sections Planned: {{count}}/{{total}}
- Page Allocation: {{allocated}}/{{limit}} pages
- Narrative Arc: {{defined|pending}}
```

#### If in Writing Phase:

```
Writing Progress:
- Sections Complete: {{count}}/{{total}}
- Word Count: {{words}}/{{target}}
- Figures/Tables: {{count}}
```

#### If in Review Phase:

```
Review Progress:
- Sections Reviewed: {{count}}/{{total}}
- Issues Found: {{critical}}/{{major}}/{{minor}}
- Revisions Complete: {{percentage}}%
```

### Timeline Analysis

Calculate and display:

- Days until deadline
- Current pace vs. required pace
- Risk assessment
- Recommended adjustments

### Warnings and Alerts

Display if applicable:

- ⚠️ Behind schedule warning
- 🚨 Deadline approaching (< 7 days)
- ❗ Blocked tasks
- 📝 Pending reviews

## Outputs

- Visual progress dashboard
- Timeline assessment
- Next action recommendations
- Quick action menu

## Integration

- Reads from paper metadata
- Tracks workflow progress
- Monitors agent activity
- Calculates timeline metrics

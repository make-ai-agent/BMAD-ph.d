# Start Paper Task

## ⚠️ CRITICAL EXECUTION NOTICE ⚠️

**THIS IS AN EXECUTABLE WORKFLOW - NOT REFERENCE MATERIAL**

When this task is invoked:

1. **TEAM COORDINATION REQUIRED** - This orchestrates multiple agents
2. **GUIDED SETUP PROCESS** - User interaction required for configuration
3. **WORKFLOW INITIALIZATION** - Kicks off the conference paper workflow

## Task Overview

This task initializes a new academic paper project, gathering essential information and launching the appropriate workflow with the Ph.D. Paper Writing Team.

## Activation

When user runs `*start-paper` command at the team level, begin this workflow immediately.

## Process

### Phase 1: Project Setup

1. **Gather Basic Information**
   - Paper ID (generate if not provided)
   - Working title (can be refined later)
   - Target conference
   - Submission deadline
   - Author information

**ELICITATION REQUIRED**: Present form for user to fill:

```
Starting new paper project...

Please provide the following information:
1. Working Title: [can be changed later]
2. Target Conference: [e.g., NeurIPS, ICML, KDD]
3. Submission Deadline: [date]
4. Lead Author: [name]
5. Research Area: [e.g., fairness in ML, computer vision]

Or type 'quick' for rapid setup with defaults.
```

### Phase 2: Conference Requirements

1. **Load Conference Template**

   - Check if conference is recognized
   - Load page limits and requirements
   - Note special sections needed

2. **Confirm Requirements**
   - Page limit: X pages
   - Blind review: Yes/No
   - Special requirements: [list]

**ELICITATION REQUIRED**: Confirm conference details or allow customization.

### Phase 3: Workspace Initialization

1. **Create Project Structure**

   ```
   papers/{paper-id}/
   ├── metadata.yaml
   ├── drafts/
   │   └── v1/
   ├── reviews/
   ├── references/
   └── figures/
   ```

2. **Initialize Metadata**
   ```yaml
   paper:
     id: { generated-id }
     title: { working-title }
     conference: { conference }
     deadline: { date }
     status: ideation
     created: { timestamp }
   ```

### Phase 4: Workflow Selection

1. **Choose Workflow Path**
   - Full paper (default): conference-paper-workflow
   - Quick review: For existing draft review
   - Literature survey: For survey papers

**ELICITATION REQUIRED**:

```
Select your starting point:
1. New Research Paper (full workflow) - Recommended
2. Review Existing Draft (quick review)
3. Literature Survey Paper (survey workflow)
4. Custom Path (specify)

Select 1-4:
```

### Phase 5: Launch Workflow

Based on selection, activate appropriate workflow:

#### For New Research Paper:

1. **Activate Researcher Agent**

   ```
   Activating Dr. Kwon (Researcher) for ideation phase...
   ```

2. **Provide Context**

   - Pass research area
   - Share conference target
   - Note any constraints

3. **Start Ideation**
   - Automatically run `*ideate {research_area}`
   - Begin research-ideation task

#### For Review Existing Draft:

1. **Activate Reviewer Agent**
2. **Request draft location**
3. **Begin review workflow**

#### For Literature Survey:

1. **Activate Researcher Agent**
2. **Configure for survey mode**
3. **Begin survey workflow**

### Phase 6: Project Tracking

1. **Register Project**

   - Add to active projects list
   - Set up progress tracking
   - Initialize timeline

2. **Provide Dashboard**

   ```
   Paper Project Initialized!

   ID: {paper-id}
   Title: {title}
   Conference: {conference}
   Deadline: {deadline} ({days} days remaining)
   Current Phase: Research Ideation
   Active Agent: Dr. Kwon (Researcher)

   Next Steps:
   - Complete ideation with researcher
   - Move to structure design
   - Begin writing phase

   Use *status to check progress anytime.
   ```

## Outputs

- Initialized paper project workspace
- Metadata file with project configuration
- Active workflow instance
- First agent activated and ready

## Error Handling

- Missing conference template: Offer to create custom
- Invalid deadline: Warn but continue
- Workspace exists: Offer to resume or create new

## Integration Points

- Hands off to conference-paper-workflow
- Activates appropriate first agent
- Sets up monitoring/tracking

## Quick Start Option

For experienced users:

```
*start-paper quick "ML Fairness" NeurIPS 2024-06-01
```

Creates project with defaults and immediately starts ideation.

# Paper Structure Design Task

## ⚠️ CRITICAL EXECUTION NOTICE ⚠️

**THIS IS AN EXECUTABLE WORKFLOW - NOT REFERENCE MATERIAL**

When this task is invoked:

1. **CONFERENCE REQUIREMENTS ARE MANDATORY** - Must align with specific conference format
2. **ELICITATION REQUIRED** - User must approve structure before proceeding
3. **PAGE LIMITS ARE HARD CONSTRAINTS** - Design must fit within limits

## Task Overview

This task creates an optimal paper structure tailored to specific conference requirements, ensuring compelling narrative flow while meeting all formatting constraints.

## Activation

When user requests paper structure design or runs `*structure` command, begin this workflow immediately.

## Inputs

- **Conference Name** (required): Target conference (e.g., NeurIPS, ICML, KDD)
- **Research Summary** (required): Core research question and approach
- **Page Limit** (required): Conference page constraints
- **Key Results** (optional): Main findings to highlight

## Process

### Phase 1: Conference Requirements Analysis

1. **Load Conference Template**

   - Page limits and formatting
   - Required sections
   - Citation style
   - Supplementary material rules

2. **Identify Special Requirements**
   - Reproducibility statements
   - Ethics statements
   - Code/data availability
   - Broader impact sections

**OUTPUT**: Conference requirements summary

### Phase 2: Content Inventory

1. **List All Content Elements**

   - Introduction hooks
   - Related work scope
   - Method components
   - Experimental setup
   - Results and analysis
   - Discussion points

2. **Estimate Space Requirements**
   - Calculate space per element
   - Identify critical vs. optional content
   - Plan for figures and tables

**ELICITATION REQUIRED**: Present content inventory with space estimates. Get user priorities.

### Phase 3: Structure Design

1. **Create Section Outline**

   ```
   1. Introduction (1.5 pages)
      - Hook and motivation
      - Problem statement
      - Contributions
      - Paper organization

   2. Related Work (1 page)
      - Categorized by approach
      - Positioning of our work

   3. Method (2.5 pages)
      - Problem formulation
      - Proposed approach
      - Algorithm details
      - Theoretical analysis

   4. Experiments (2 pages)
      - Setup and datasets
      - Baselines
      - Results
      - Ablations

   5. Discussion (0.5 pages)
      - Implications
      - Limitations

   6. Conclusion (0.5 pages)
   ```

2. **Design Narrative Arc**
   - Opening hook strategy
   - Building tension/problem
   - Solution revelation
   - Evidence presentation
   - Impact emphasis

**ELICITATION REQUIRED**: Present structure with narrative flow. Allow user modifications.

### Phase 4: Space Optimization

1. **Allocation Strategy**

   - Must-have content
   - Nice-to-have content
   - Supplementary candidates

2. **Compression Techniques**

   - Bullet points vs. prose
   - Figure combinations
   - Table condensation
   - Appendix usage

3. **Create Contingency Plans**
   - If over limit: what to cut
   - If under limit: what to expand

**ELICITATION REQUIRED**: Present final structure with contingencies. Get approval.

### Phase 5: Writing Guidelines

1. **Section-Specific Guidance**

   - Key points per section
   - Transition strategies
   - Technical depth targets

2. **Style Guidelines**
   - Active vs. passive voice
   - Technical terminology usage
   - Figure/table references

## Outputs

- **Structure Document** containing:
  - Detailed section outline
  - Space allocations
  - Content priorities
  - Narrative flow plan
  - Writing guidelines
  - Conference compliance checklist

## Collaboration Points

- **With Architect Agent**: For technical content organization
- **With Writer Agent**: For prose planning
- **With Reviewer Agent**: For compliance verification

## Quality Criteria

- Conference compliance
- Narrative coherence
- Space efficiency
- Technical completeness
- Reader engagement

## Common Pitfalls to Avoid

- Exceeding page limits
- Weak introduction hooks
- Imbalanced sections
- Missing required elements
- Poor figure/text balance

# Content Review Task

## ⚠️ CRITICAL EXECUTION NOTICE ⚠️

**THIS IS AN EXECUTABLE WORKFLOW - NOT REFERENCE MATERIAL**

When this task is invoked:

1. **RIGOROUS STANDARDS REQUIRED** - Apply peer-review level scrutiny
2. **CONSTRUCTIVE FEEDBACK MANDATORY** - Provide actionable improvements
3. **MULTIPLE PASSES EXPECTED** - Iterative refinement is normal

## Task Overview

This task performs comprehensive academic content review, ensuring research quality, methodological rigor, and adherence to academic standards.

## Activation

When user requests content review or runs `*review` command, begin this workflow immediately.

## Inputs

- **Section/Document** (required): Content to review
- **Review Type** (required): methodology/technical/clarity/comprehensive
- **Conference Standards** (optional): Specific conference requirements
- **Review Criteria** (optional): Custom focus areas

## Process

### Phase 1: Initial Assessment

1. **Quick Read-Through**

   - Understand main claims
   - Note immediate concerns
   - Assess overall structure

2. **Categorize Issues**
   - Critical (must fix)
   - Major (should fix)
   - Minor (nice to fix)
   - Suggestions (optional)

**OUTPUT**: Initial assessment summary

### Phase 2: Detailed Technical Review

1. **Methodology Validation**

   - Is the approach sound?
   - Are assumptions stated?
   - Is the experimental design valid?
   - Are controls appropriate?

2. **Technical Accuracy**

   - Check mathematical formulations
   - Verify algorithm descriptions
   - Validate complexity analyses
   - Confirm technical claims

3. **Results Verification**
   - Are results clearly presented?
   - Do numbers add up?
   - Are comparisons fair?
   - Is statistical significance shown?

**ELICITATION REQUIRED**: Present technical issues with severity ratings. Get author response.

### Phase 3: Academic Writing Review

1. **Clarity and Flow**

   - Is the narrative clear?
   - Do paragraphs connect logically?
   - Are concepts well-explained?
   - Is jargon appropriate?

2. **Academic Conventions**

   - Proper citation format
   - Figure/table references
   - Notation consistency
   - Tense usage

3. **Argument Structure**
   - Claims supported by evidence
   - Logical progression
   - Appropriate hedging
   - Balanced discussion

**ELICITATION REQUIRED**: Present writing improvements with examples. Get preferences.

### Phase 4: Reproducibility Check

1. **Method Description**

   - Sufficient implementation details?
   - Hyperparameters specified?
   - Data preprocessing clear?
   - Evaluation metrics defined?

2. **Resource Requirements**
   - Computational needs stated?
   - Dataset availability?
   - Code availability plans?

**OUTPUT**: Reproducibility assessment

### Phase 5: Final Recommendations

1. **Priority Action Items**

   - List must-fix issues
   - Suggest fix strategies
   - Estimate effort required

2. **Enhancement Opportunities**

   - Ways to strengthen paper
   - Additional experiments
   - Presentation improvements

3. **Overall Assessment**
   - Ready for submission?
   - Major revision needed?
   - Minor revision needed?

**ELICITATION REQUIRED**: Present final recommendations. Plan revision strategy.

## Review Checklist Template

```markdown
## Technical Review

- [ ] Methodology is sound
- [ ] Assumptions are stated
- [ ] Experiments are well-designed
- [ ] Results support claims
- [ ] Limitations acknowledged

## Writing Quality

- [ ] Clear and concise
- [ ] Proper academic tone
- [ ] Good narrative flow
- [ ] Consistent terminology
- [ ] Proper citations

## Reproducibility

- [ ] Method fully described
- [ ] Parameters specified
- [ ] Data sources clear
- [ ] Code availability stated

## Conference Compliance

- [ ] Within page limits
- [ ] Required sections present
- [ ] Formatting correct
- [ ] Supplementary appropriate
```

## Outputs

- **Review Report** containing:
  - Executive summary
  - Detailed findings by category
  - Prioritized action items
  - Suggested improvements
  - Overall recommendation

## Collaboration Points

- **With Writer Agent**: For implementing fixes
- **With Paper Expert**: For structural changes
- **With Researcher**: For methodology questions

## Quality Criteria

- Thoroughness
- Constructiveness
- Actionability
- Academic rigor
- Fairness

## Common Review Focus Areas

- Overclaimed results
- Insufficient baselines
- Cherry-picked results
- Unclear methodology
- Poor literature coverage
- Weak motivation
- Missing limitations

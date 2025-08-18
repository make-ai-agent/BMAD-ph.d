# Academic Writing Task

## ⚠️ CRITICAL EXECUTION NOTICE ⚠️

**THIS IS AN EXECUTABLE WORKFLOW - NOT REFERENCE MATERIAL**

When this task is invoked:

1. **SECTION-BY-SECTION APPROACH** - Write incrementally with feedback
2. **TECHNICAL ACCURACY PARAMOUNT** - Collaborate with domain experts
3. **ITERATIVE REFINEMENT EXPECTED** - First drafts are never final

## Task Overview

This task guides the academic writing process for conference papers, ensuring clear technical communication while maintaining engagement and meeting strict space constraints.

## Activation

When user requests writing assistance or runs `*write` command, begin this workflow immediately.

## Inputs

- **Section to Write** (required): Which part of the paper
- **Outline/Notes** (required): Key points to cover
- **Space Limit** (required): Available pages/words
- **Technical Details** (optional): Formulas, algorithms, results
- **Style Preferences** (optional): Conference-specific style

## Process

### Phase 1: Pre-Writing Setup

1. **Review Section Requirements**

   - Purpose of this section
   - Key messages to convey
   - Connection to other sections
   - Space constraints

2. **Gather Technical Content**
   - Collect formulas/algorithms
   - Prepare figures/tables
   - List key citations
   - Note terminology choices

**OUTPUT**: Writing plan with key elements

### Phase 2: Draft Creation

#### For Introduction Section:

1. **Opening Hook** (2-3 sentences)

   - Start with impact/importance
   - Or start with surprising fact
   - Or start with key challenge

2. **Problem Context** (1 paragraph)

   - Why this matters now
   - Current limitations
   - Stakes involved

3. **Specific Problem** (1 paragraph)

   - Technical problem definition
   - Why it's hard
   - Previous attempts

4. **Our Approach** (1 paragraph)

   - Key insight
   - High-level solution
   - Why it works

5. **Contributions** (Bullet list)
   - Specific, measurable claims
   - What's novel
   - Impact achieved

**ELICITATION REQUIRED**: Present draft introduction. Get feedback on hook and flow.

#### For Method Section:

1. **Problem Formulation**

   - Notation definitions
   - Formal problem statement
   - Assumptions

2. **Approach Overview**

   - Intuition first
   - High-level algorithm
   - Key innovations

3. **Technical Details**

   - Step-by-step algorithm
   - Theoretical properties
   - Complexity analysis

4. **Implementation Notes**
   - Practical considerations
   - Optimization tricks
   - Parameter choices

**ELICITATION REQUIRED**: Present technical writing. Verify clarity and correctness.

#### For Results Section:

1. **Experimental Setup**

   - Datasets description
   - Evaluation metrics
   - Baseline methods
   - Implementation details

2. **Main Results**

   - Lead with best results
   - Clear comparisons
   - Statistical significance

3. **Analysis**

   - Why method works
   - When it fails
   - Ablation studies

4. **Visualizations**
   - Figure design
   - Caption writing
   - In-text references

**ELICITATION REQUIRED**: Present results narrative. Ensure compelling story.

### Phase 3: Technical Prose Refinement

1. **Clarity Passes**

   - Simplify complex sentences
   - Define before use
   - Add intuition
   - Use examples

2. **Precision Passes**

   - Check technical accuracy
   - Verify terminology
   - Confirm notation
   - Fix ambiguities

3. **Flow Passes**
   - Smooth transitions
   - Logical progression
   - Paragraph connections
   - Section coherence

**ELICITATION REQUIRED**: Show refined version. Get approval or iterate.

### Phase 4: Space Optimization

1. **Compression Techniques**

   - Combine related points
   - Use active voice
   - Remove redundancy
   - Tighten prose

2. **Strategic Cuts**
   - Move to appendix
   - Combine figures
   - Summarize details
   - Reference instead of repeat

**OUTPUT**: Space-optimized version

### Phase 5: Polish and Finalize

1. **Citation Integration**

   - Smooth incorporations
   - Proper grouping
   - Recent works

2. **Final Checks**
   - Consistent terminology
   - Notation consistency
   - Figure/table refs
   - No dangling references

## Writing Patterns by Section

### Introduction Patterns

```
"Recent advances in X have enabled Y, yet Z remains challenging..."
"While X has shown promise for Y, existing methods fail when..."
"The key insight of our work is that..."
"We make the following contributions:"
```

### Method Patterns

```
"Formally, we define the problem as..."
"The key intuition behind our approach is..."
"Algorithm 1 summarizes our procedure..."
"The complexity of our method is O(...) because..."
```

### Results Patterns

```
"Table 1 shows that our method consistently..."
"As shown in Figure 2, we observe that..."
"These results demonstrate that..."
"The improvement can be attributed to..."
```

## Outputs

- **Written Section** containing:
  - Polished prose
  - Integrated figures/tables
  - Proper citations
  - Smooth transitions
  - Technical accuracy

## Collaboration Points

- **With Dev Agent**: For implementation details
- **With Researcher**: For technical accuracy
- **With Reviewer**: For clarity checks

## Quality Criteria

- Technical accuracy
- Clarity for target audience
- Engaging narrative
- Proper academic tone
- Space efficiency

## Common Writing Pitfalls

- Burying the lead
- Overwhelming with details
- Weak transitions
- Passive voice overuse
- Undefined terminology
- Vague claims
- Missing intuition

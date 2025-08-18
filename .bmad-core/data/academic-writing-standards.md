# Academic Writing Standards

## Purpose

Standards and guidelines for high-quality academic writing in data science papers.

## Clarity and Precision

### Technical Terminology

- **First Use**: Define technical terms on first use
- **Consistency**: Use the same term throughout (don't alternate between synonyms)
- **Notation**: Introduce mathematical notation before using
- **Acronyms**: Spell out on first use, then use consistently

### Sentence Structure

- **Active Voice**: Prefer "We propose..." over "It is proposed..."
- **Conciseness**: Eliminate unnecessary words
- **Parallel Structure**: Use consistent grammatical patterns in lists
- **Clarity**: One main idea per sentence

### Paragraph Structure

- **Topic Sentence**: Start with the main point
- **Supporting Evidence**: Follow with evidence/explanation
- **Transition**: Connect to next paragraph
- **Length**: Typically 3-6 sentences

## Mathematical Writing

### Equation Standards

- **Variables**: Define all variables immediately
- **Numbering**: Number equations referenced in text
- **Punctuation**: Treat equations as part of sentences
- **Alignment**: Align multi-line equations properly

### Notation Guidelines

- **Consistency**: Same symbol = same meaning throughout
- **Convention**: Follow field conventions (e.g., bold for vectors)
- **Clarity**: Avoid similar-looking symbols
- **Sets**: Use standard set notation

### Example Format

```
We define the loss function as:
    L(θ) = Σᵢ ℓ(yᵢ, f(xᵢ; θ)) + λR(θ)    (1)
where ℓ is the loss function, R(θ) is the regularization term,
and λ controls the regularization strength.
```

## Citation Standards

### When to Cite

- **Ideas**: Any idea not your own
- **Methods**: Algorithms, techniques, approaches
- **Data**: Datasets, benchmarks
- **Facts**: Statistics, findings from other work
- **Quotes**: Any direct quotations

### Citation Placement

- **End of Sentence**: Most common placement
- **Mid-Sentence**: When needed for clarity
- **Multiple Works**: Group related citations [1, 2, 3]
- **Page Numbers**: For specific claims or quotes

### Citation Verbs

- **Neutral**: "Smith et al. [1] present..."
- **Positive**: "Successfully demonstrated [1]..."
- **Contrasting**: "Unlike [1], we..."
- **Building**: "Extending [1], we..."

## Academic Tone

### Professional Language

- **Formal**: Avoid colloquialisms and slang
- **Objective**: Focus on evidence, not opinions
- **Precise**: Use specific rather than general terms
- **Modest**: Avoid hyperbole and overstatement

### Appropriate Hedging

- **Certainty Levels**:
  - High: "demonstrate", "prove", "establish"
  - Medium: "indicate", "suggest", "support"
  - Low: "may", "might", "could"

### Common Phrases

- ✅ "The results indicate..."
- ❌ "The results clearly prove without doubt..."
- ✅ "Our method achieves competitive performance"
- ❌ "Our method is the best"

## Figure and Table Standards

### Captions

- **Self-Contained**: Understandable without main text
- **Descriptive**: What, not just where
- **Details**: Include important parameters
- **References**: Cite if adapted from other work

### References in Text

- **Explicit**: "As shown in Figure 1..."
- **Purposeful**: Explain what reader should notice
- **Timely**: Reference before or as appears
- **Complete**: Reference all figures/tables

### Quality Guidelines

- **Resolution**: High quality, readable text
- **Consistency**: Same style throughout paper
- **Accessibility**: Consider color-blind readers
- **Simplicity**: Remove unnecessary elements

## Ethics in Writing

### Plagiarism Avoidance

- **Paraphrasing**: Fully rewrite in your words
- **Quotations**: Use sparingly, with quotes
- **Self-Plagiarism**: Don't reuse own text
- **Attribution**: Always give credit

### Result Reporting

- **Honesty**: Report all results, not just positive
- **Transparency**: Describe failures and limitations
- **Reproducibility**: Provide all necessary details
- **Statistical Rigor**: Use appropriate tests

### Authorship

- **Contribution**: All authors must contribute
- **Order**: Reflect relative contributions
- **Acknowledgments**: Credit other helpers
- **Conflicts**: Disclose any conflicts of interest

## Common Errors to Avoid

### Grammar and Style

- ❌ "The method it works by..."
- ✅ "The method works by..."
- ❌ "e.g." in text
- ✅ "for example" or "(e.g., ...)"
- ❌ Starting with "However, ..."
- ✅ Embedding "however" in sentence

### Technical Writing

- ❌ "The algorithm is very fast"
- ✅ "The algorithm runs in O(n log n) time"
- ❌ "Results improve a lot"
- ✅ "Results improve by 23.5%"
- ❌ Undefined abbreviations
- ✅ All abbreviations defined on first use

### Logic and Flow

- ❌ Jumping between topics
- ✅ Logical progression of ideas
- ❌ Assuming reader knowledge
- ✅ Providing necessary background
- ❌ Circular reasoning
- ✅ Clear cause-and-effect

## Review Checklist

Before submission, ensure:

- [ ] All technical terms defined
- [ ] Consistent notation throughout
- [ ] All citations complete and formatted
- [ ] Figures/tables referenced and explained
- [ ] No grammatical errors
- [ ] Appropriate academic tone
- [ ] Claims match evidence
- [ ] Limitations acknowledged

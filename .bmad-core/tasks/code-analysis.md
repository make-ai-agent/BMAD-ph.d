# code-analysis

## Task Overview

This task enables Dr. Im (Code Analyst) to perform comprehensive analysis of code implementations and translate technical details into academic paper format. The task focuses on ensuring technical accuracy and bridging the gap between code implementation and theoretical description.

## Activation

This task is activated when:
- User requests code analysis or implementation explanation
- Paper sections need technical implementation details
- Verification of paper claims against actual code is needed
- Repository synchronization is required

## Prerequisites

- Access to `./code` directory or specified code repository
- Git repository access for latest version synchronization
- Understanding of the research method being implemented

## Process

### Step 1: Repository and Code Assessment

```yaml
inputs:
  - target_repository: URL or path to code repository
  - code_directory: ./code (default) or specified path
  - focus_area: specific method, file, or component to analyze
  - analysis_depth: high-level | detailed | comprehensive

actions:
  - Verify repository access and latest version
  - Scan code directory structure
  - Identify main implementation files
  - Check for documentation and comments
```

### Step 2: Code Implementation Analysis

```yaml
analysis_framework:
  architecture_review:
    - Overall code organization and structure
    - Key classes, functions, and modules
    - Design patterns and architectural choices
    - Dependencies and external libraries
  
  algorithm_analysis:
    - Core algorithm implementation
    - Mathematical operations and computations
    - Data flow and processing pipeline
    - Optimization techniques used
  
  method_implementation:
    - Proposed method implementation details
    - Parameter handling and configuration
    - Input/output specifications
    - Error handling and edge cases

outputs:
  - Implementation overview document
  - Algorithm flowchart or diagram
  - Key code snippets with explanations
  - Technical specifications summary
```

### Step 3: Academic Translation

```yaml
academic_formatting:
  method_description:
    - Translate code logic into academic prose
    - Create mathematical notation from code
    - Explain algorithm steps clearly
    - Provide implementation details section
  
  technical_accuracy:
    - Verify claims against actual implementation
    - Check performance characteristics
    - Validate experimental setup
    - Ensure reproducibility information
  
  documentation_generation:
    - Create pseudocode representations
    - Generate technical diagrams
    - Provide code examples
    - Write implementation notes

collaboration_points:
  with_researcher:
    - Validate theoretical foundation against code
    - Identify implementation insights for research
  with_writer:
    - Provide technical content for method sections
    - Review technical writing accuracy
  with_reviewer:
    - Verify implementation claims
    - Check technical completeness
```

### Step 4: Quality Assurance and Verification

```yaml
verification_checklist:
  - ✓ Code analysis matches paper description
  - ✓ All technical claims are implementation-backed
  - ✓ Mathematical formulations align with code
  - ✓ Performance characteristics are accurate
  - ✓ Reproducibility information is complete
  - ✓ Latest repository version is referenced

output_standards:
  - Technical accuracy: 100%
  - Implementation coverage: Comprehensive
  - Academic clarity: High
  - Reproducibility: Complete
```

## Outputs

### Primary Deliverables

1. **Implementation Analysis Report**
   - Code structure overview
   - Algorithm implementation details
   - Technical specifications
   - Performance characteristics

2. **Academic Method Description**
   - Formal method description
   - Mathematical notation
   - Algorithm pseudocode
   - Implementation details section

3. **Technical Verification Document**
   - Claim-to-code verification
   - Accuracy assessment
   - Reproducibility checklist
   - Repository information

### Supporting Materials

- Code documentation
- Technical diagrams
- Performance benchmarks
- Implementation notes

## Integration Points

### With Research Process
- Validate theoretical concepts against implementation
- Identify code-based research insights
- Ensure implementation feasibility

### With Writing Process
- Provide accurate technical descriptions
- Supply code examples and explanations
- Review technical sections for accuracy

### With Review Process
- Verify technical claims
- Check implementation completeness
- Validate reproducibility

## Success Criteria

- Technical descriptions accurately reflect code implementation
- All claims are verifiable through code analysis
- Implementation details are clearly explained
- Repository synchronization is maintained
- Academic and technical standards are met

## Notes

- Always work with the latest repository version
- Maintain focus on pedagogical clarity
- Ensure technical accuracy over simplification
- Bridge theory-implementation gap effectively
- Support reproducible research practices
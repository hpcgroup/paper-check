# Paper-Check: Academic Paper Quality Checking Tool

## 1. Design Philosophy

Paper-Check is an automated paper quality checking tool designed to help academic authors improve paper quality. Its core design philosophy includes:

- **Comprehensive Checking**: Combines static analysis and Large Language Model (LLM) evaluation to check both paper format and content quality
- **Multi-dimensional Assessment**: Evaluates papers across multiple dimensions including titles, section layout, figures, writing style, etc.
- **Automated Reporting**: Generates detailed quality reports that clearly identify issues and provide improvement suggestions
- **Dual Input Sources**: Analyzes both PDF and LaTeX source files simultaneously to ensure comprehensive problem detection

## 2. Checking Items

### Static Checks (Rule-based):

- **Title Check**: Confirms whether the paper has a title and evaluates title descriptiveness
- **Section Title Check**:
  - Title descriptiveness and content relevance
  - Correct capitalization format (Title Case)
- **Section Buffer**: Checks if there is sufficient buffer between sections (avoiding overcrowding)
- **Figure Check**:
  - Presence of figure titles and labels
  - Correct figure references
  - Adequacy of figure descriptions
- **Number Spelling**: Checks correct spelling of numbers (e.g., whether numbers less than 10 should be written as words)
- **Informal Wording**: Detects informal or inappropriate words for academic writing
- **Italics Usage**: Checks correct use of italics for terms, variables, etc.

### LLM Evaluation (Large Language Model-based):

- **Title Evaluation**: Evaluates the quality, relevance, and coherence of the title and section titles
- **Introduction Evaluation**: Analyzes the completeness, clarity, and purposefulness of the introduction
- **Writing Quality**: Assesses writing style, clarity, and academic nature of each section
- **Figure Visual Evaluation**: Uses visual analysis capabilities to evaluate the clarity and effectiveness of figures

## 3. Writing Principles

By using Paper-Check, you can follow these academic writing principles:

- **Clarity**: Titles and content should clearly express research focus and findings
- **Structure**: Paper structure should be logically clear with natural transitions between sections
- **Formality**: Use formal academic language, avoiding colloquialisms or informal expressions
- **Precision**: Figures should accurately express data, and terminology should be accurate and consistent
- **Completeness**: Each section should comprehensively cover necessary content without key omissions
- **Citation Standards**: Correctly cite references and related work

## 4. Usage

```bash
python paper_check.py --pdf path/to/your/paper.pdf --latex path/to/your/latex/source
```


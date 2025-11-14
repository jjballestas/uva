# UVA Academic Projects - AI Assistant Guidelines

## Project Overview

This repository contains academic coursework from Universidad de Valladolid's Master in Computer Engineering (MUIF), specifically for advanced data analysis and interaction design courses. The codebase consists of two main academic projects:

### 1. SIA (Advanced Interaction Systems Design) - `sia/`
A comprehensive interaction design project developing "SmartSound," an intelligent audio calibration system for live music performances. This project follows the double diamond design methodology with extensive user research, prototyping, and evaluation planning.

### 2. Data Science Classifiers - `clasificadores/`
Machine learning coursework focused on scalable data analysis using Apache Spark and decision trees for the Census Income (KDD) dataset classification problem.

## Key Architecture Patterns

### Document Structure Convention
- **LaTeX Academic Reports**: Both projects use LaTeX with APA7 formatting for academic documentation
- **Bilingual Content**: All documents are in Spanish with English technical references
- **Asset Organization**: Images and supporting materials stored in `assets/` subdirectories
- **Bibliography Management**: Uses BibTeX with separate `.bib` files for references

### SIA Project Workflow
- **Research Phase**: Contextual inquiry, user interviews, and thematic analysis
- **Design Phase**: Persona creation, empathy mapping, journey mapping, and scenario development  
- **Evaluation Phase**: Wizard of Oz prototyping with controlled usability testing
- **Documentation**: Structured around double diamond methodology phases

### Data Science Project Workflow
- **Data Processing**: Scala-based Apache Spark ML pipelines with feature engineering
- **Model Selection**: Systematic hyperparameter exploration using validation splits
- **Evaluation**: Multi-metric analysis including confusion matrices, AUC-ROC, and AUC-PR
- **Documentation**: Technical reports with code snippets and visual analysis

## Development Workflows

### LaTeX Compilation
Projects use MiKTeX on Windows with automatic PDF generation:
```bash
# Standard LaTeX compilation workflow
pdflatex main.tex
bibtex main
pdflatex main.tex  
pdflatex main.tex
```

### Asset Management
- Images referenced as `./assets/filename.extension`
- UVA logo consistently used across projects: `./assets/uva-logo.png`
- Research photos and analysis diagrams stored per project

## Critical Project-Specific Knowledge

### SIA Project Context
- **Target Users**: Musicians (3-5 member bands) performing without dedicated sound technicians
- **Core Problem**: Audio self-management difficulties during live performances in bars/small venues
- **Solution Approach**: Smart audio calibration system with real-time monitoring
- **Research Methods**: Contextual inquiry in Valladolid music venues (Caimanes del Esgueva, Cañoneros, Arowana)
- **Key Findings**: Professional bands with sound engineers excluded as target users

### Data Science Project Context  
- **Dataset**: Census Income (KDD) with 299,285 records, highly imbalanced classes (93.8% vs 6.2%)
- **Challenge**: Predicting income >$50K using demographic and employment features
- **Method**: Decision tree classification with maxDepth/maxBins parameter exploration
- **Best Model**: maxDepth=10, maxBins=100 achieving 5.96% error rate
- **Key Issue**: Low recall (42%) for minority class detection

## Conventions and Standards

### File Naming
- Main documents always named `main.tex`
- Asset files use descriptive lowercase names with hyphens
- Bibliography files: `refs.bib` (SIA), `main.bib` (Classificadores)

### Content Structure
- Title pages with UVA branding and course information
- Table of contents with Spanish section names
- Figure captions in Spanish with proper referencing using `cleveref`
- Academic year format: "2025 -- 2026"

### Citation Style
- APA7 style throughout both projects
- Online sources include access dates ("Acceso: [date]")
- Technical documentation properly cited (Spark API, Nielsen Norman Group)

## When Working on These Projects

1. **Maintain Academic Integrity**: These are coursework submissions - respect academic standards
2. **Spanish Language**: All narrative content should be in Spanish 
3. **Consistent Formatting**: Follow established LaTeX templates and UVA branding
4. **Evidence-Based**: SIA project requires user research citations; Data Science project requires metric validation
5. **Professional Presentation**: Both projects emphasize rigorous methodology and clear documentation

## External Dependencies

- **MiKTeX**: LaTeX distribution for document compilation
- **Apache Spark**: Required for data science project implementation  
- **Miro**: Used for collaborative design work (SIA project)
- **Figma**: Prototyping tool mentioned for evaluation planning
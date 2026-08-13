# When Tests Need Judgement: Agentic AI and the Future of New Feature Testing

This repository contains the LaTeX source files for the paper **“When Tests Need Judgement: Agentic AI and the Future of New Feature Testing”**

The paper presents a conceptual framework for using agentic artificial intelligence in software quality assurance, with a specific focus on **new feature testing**. It argues that agentic AI should not be treated as a replacement for human testers or deterministic regression automation. Instead, it should be positioned as a **human-supervised exploratory testing partner** in contexts where requirements are evolving, expected outcomes are incomplete, and oracle validation requires human judgement.

## Manuscript Summary

Agentic AI systems can plan actions, interact with software environments, observe outcomes, adapt subsequent steps, and produce evidence. These capabilities create opportunities for software testing, but they also raise questions about responsibility, accountability, and trust.

This paper addresses the following central question:

> How can agentic AI support new feature testing while preserving human responsibility for exploratory judgement, oracle validation, and release confidence?

The proposed answer is a **responsibility-oriented framework** organised around five phases:

1. **Preparation**  
   Humans define the testing mission, scope, risk focus, data rules, and prohibited actions.

2. **Exploration**  
   The agent may explore supervised UI or API paths, vary inputs, and exercise workflows.

3. **Observation**  
   The agent captures evidence such as screenshots, logs, payloads, timestamps, and action traces.

4. **Interpretation**  
   Humans validate expected outcomes, classify defects, assess severity, and interpret requirement ambiguity.

5. **Governance**  
   Human reviewers retain accountability through traceability, evidence review, permission control, and release decision authority.

## Main Contributions

The paper makes the following contributions:

- Defines the role of agentic AI in new feature testing.
- Distinguishes agentic AI from deterministic regression automation and static LLM-based test generation.
- Proposes a five-phase responsibility-oriented framework for supervised agentic AI in feature-level QA.
- Identifies governance mechanisms for traceability, reviewability, data handling, and accountability.
- Proposes an empirical validation agenda comparing manual exploratory testing, static LLM-assisted testing, supervised agentic AI, and deterministic automation.

## Repository Structure

```text
.
├── conference.tex          # Main conference paper source
├── references.bib          # Optional BibTeX references, if used
├── figures/                # Optional figures and diagrams
├── README.md               # Repository description
└── LICENSE                 # License file, if applicable
```

If the paper uses an inline IEEE-style bibliography, the references are included directly in `conference.tex` using:

```latex
\begin{thebibliography}{00}
...
\end{thebibliography}
```

## How to Compile

To compile the paper locally, use a LaTeX distribution such as TeX Live, MiKTeX, or Overleaf.

### Option 1: Compile with PDFLaTeX

```bash
pdflatex conference.tex
pdflatex conference.tex
```

### Option 2: Compile with Overleaf

1. Create a new Overleaf project.
2. Upload `conference.tex` and any required figure files.
3. Set `conference.tex` as the main file.
4. Compile using PDFLaTeX.

## Citation

If you use or refer to this work, please cite it as:

```bibtex
@misc{otano2026agentic,
  author = {Otano, Paula Soledad and Rodriguez Rivero, Cristian},
  title = {When Tests Need Judgement: Agentic AI and the Future of New Feature Testing},
  journal = {Software Quality Journal},
  year = {2026},
  note = {Manuscript}
}
```

## Keywords

- Agentic AI
- Software Quality Assurance
- New Feature Testing
- Exploratory Testing
- Human-AI Collaboration
- Test Oracle
- Human-AI Trust
- Software Testing Governance

## Status

This repository contains a conceptual research paper. The proposed framework has not yet been empirically validated. Future work should include expert review, controlled experiments, replication studies, and industrial case studies.

## Authors

**Paula Soledad Otano**  
Systems Engineering  
National University of Technology, UTN-FRC  
Cordoba, Argentina  

**Cristian Rodriguez Rivero**  
Department of Mechatronics  
Fontys University of Applied Sciences  
Eindhoven, The Netherlands  

## License

Please add the appropriate license for this repository. For academic manuscripts, common choices include:

- `CC BY 4.0` for open academic sharing
- `MIT License` for reusable code or templates
- No license, if reuse is not currently permitted

## Disclaimer

This repository is intended for academic and research purposes. The framework described in the paper should be interpreted as a conceptual model and validation agenda, not as empirical proof that agentic AI improves software testing outcomes.
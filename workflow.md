# 从结果图和背景资料写成完整论文初稿的可复用流程

This document captures the workflow used to transform scattered source materials, six main figures, supplementary files, and user corrections into complete English and Chinese biomedical manuscript drafts. It is intended as a reusable operating procedure for future figure-led manuscript writing projects.

## 1. 任务目标

The goal is not to "polish a draft" in the narrow sense. The goal is to reconstruct the complete paper from evidence:

- Read all figures and source files.
- Recover what each figure panel proves.
- Connect the evidence into a coherent scientific story.
- Write a complete manuscript with deep Introduction, detailed Results, formal Materials and Methods, full figure legends, and a mature Discussion.
- Produce bilingual versions when needed.
- Avoid the common failure mode where an initial AI draft sounds fluent but drops essential experimental details.

The correct output is a manuscript that a domain researcher can continue editing, not a generic review-like text.

## 2. 输入材料清单

For each project, create an inventory before writing:

| Material type | What to extract | Why it matters |
| --- | --- | --- |
| Main figures | Panel labels, assay type, group names, quantitative values, pathway names, imaging content | Determines Results structure and figure legends |
| Original manuscript or old draft | Existing wording, references, methods, figure explanations | Prevents loss of source information |
| Rewritten draft | Current structure and prose quality | Provides a base but must be audited for omissions |
| Supplementary materials | Tables, instrument parameters, extra figures, target lists, metabolite lists | Supplies Methods and detailed Results |
| Reference PDF | Section layout, paragraph depth, caption style, Methods granularity | Provides target publication standard |
| User corrections | Doses, units, ethics number, modeling conditions, instrument models, calibration ranges | Overrides uncertain or missing draft content |

Do not start by writing prose. Start by building the evidence map.

## 3. 图证据台账

Create a figure-panel evidence ledger. This is the central anti-omission device.

Recommended columns:

| Figure panel | What is shown | Source file or source section | Key details to preserve | Manuscript location |
| --- | --- | --- | --- | --- |
| Fig. 1A | Experimental timeline or model design | Main figure/source draft | Age, model reagent, treatment time, dose range | Results + Methods + legend |
| Fig. 1B-D | Behavioral or biochemical outcomes | Main figure/source draft | Groups, direction of change, significance, exact values if available | Results |
| Fig. 2A-G | Distribution and AFADESI-MSI workflow/images | Main figure/source draft | Cy3-rutin timing, tissues, m/z values, ion mode, abbreviations | Results + legend + Methods |
| Fig. 3A-I | Transcriptomics/network pharmacology | Main figure/source draft | DEG counts, GO/KEGG terms, target number, pathway names | Results + Discussion |
| Fig. 4A-F | Untargeted metabolomics | Main figure/source draft/SI | OPLS-DA/PCA, differential classes, pathway enrichment | Results |
| Fig. 5A-D | Targeted metabolomics/lipidomics | Main figure/source draft/SI | Shared metabolites/lipids, classes, concentration or trend | Results + Methods |
| Fig. 6A-H | Spatial metabolomics and integrated mechanism | Main figure/source draft | Anatomical regions, neurotransmitters, amino acids, lipid-inflammatory ions | Results + Discussion |

The exact panels will change by project. The rule does not: every panel gets mapped before writing.

## 4. 故事线构建

A strong biomedical paper needs a causal-feeling evidence sequence even when the study is mechanistic and associative.

For a figure-led natural product and disease-model paper, a robust story often follows this order:

1. **Problem and model**: establish the disease-like phenotype and intervention design.
2. **Pharmacodynamic rescue**: show the compound improves behavior, biochemical markers, pathology, or viability.
3. **Exposure and localization**: show the compound or related signal reaches relevant tissues.
4. **Unbiased discovery**: use transcriptomics/metabolomics/lipidomics to identify molecular modules.
5. **Targeted validation**: validate selected metabolite or lipid branches.
6. **Spatial anchoring**: localize molecules to anatomical regions to avoid a purely homogenate-based mechanism.
7. **Integrated mechanism**: present the mechanism as a supported network, not a single oversimplified pathway.

For the rutin-zebrafish AD manuscript, the central story became:

Rutin ameliorates AlCl3/D-gal-induced AD-like injury in zebrafish. Its effect is supported by behavioral and biochemical rescue, distribution of rutin-related signals in brain and peripheral tissues, transcriptomic enrichment of amino-acid and neurotransmitter-related pathways, metabolomic and lipidomic remodeling, and AFADESI-MSI spatial localization. The strongest mechanism is not a single alanine-only pathway but a coupled amino acid-neurotransmitter, lipid-inflammatory, and energy-metabolic network.

## 5. 初稿骨架

Before writing prose, define the article structure:

1. Title
2. Abstract
3. Keywords
4. Introduction
5. Results
   - Result section 1 + Fig. 1 + legend
   - Result section 2 + Fig. 2 + legend
   - Continue in figure order
6. Discussion
7. Materials and Methods
8. References
9. Supplementary materials, if required

When the target example places images after each result, follow that layout: result text first, then figure, then figure legend.

## 6. 经典四段式前言

A mature Introduction should usually use four paragraphs:

### Paragraph 1: Field problem and disease logic

Define the disease/problem at a high conceptual level. Include why existing frameworks are insufficient.

For AD-type studies, do not stop at amyloid or cholinergic dysfunction. A deeper paragraph should connect amyloid, tau, synaptic dysfunction, neuroinflammation, mitochondrial stress, vascular dysfunction, immune regulation, lipid metabolism, and systemic metabolism where relevant.

### Paragraph 2: Candidate intervention and knowledge gap

Introduce the compound, material, treatment, or intervention. Summarize prior evidence, then identify what remains unresolved.

For natural products, key gaps often include:

- Whole-organism distribution is unknown.
- Brain versus peripheral contribution is unclear.
- Studies focus on isolated endpoints rather than system-level mechanisms.
- Omics findings lack targeted or spatial validation.

### Paragraph 3: Model and technology rationale

Explain why the selected model and technologies are appropriate.

Include model conditions when known, for example:

- `150 μM AlCl3 + 40 mg/mL D-gal for 72 h`
- Zebrafish developmental stage or adult exposure model
- Behavioral assays
- Fluorescence tracing
- UHPLC-MS/MS
- AFADESI-MSI
- Transcriptomics, metabolomics, lipidomics, network pharmacology

### Paragraph 4: Study aim and novelty

End by stating what the study tests and what evidence chain it builds. Do not overclaim causality. A good final paragraph explains the study questions and the integrated logic.

Example question sequence:

- Does the compound produce pharmacodynamic rescue?
- Does compound-related signal reach relevant tissues?
- Which molecular modules are repeatedly supported across independent datasets?

## 7. 结果写作规则

Results must be written figure by figure and panel by panel. Avoid vague summaries such as "Fig. 2 shows distribution." Instead, write what each panel contributes.

A result section should include:

- Experimental purpose.
- What panels A, B, C, etc. show.
- Direction of change.
- Quantitative values and significance, when available.
- Interpretation limited to what the data support.
- Transition to the next figure.

Bad pattern:

> The metabolomics results showed many differential metabolites and enriched pathways.

Better pattern:

> Untargeted metabolomics was used to determine whether rutin reshaped the model-associated metabolic phenotype. The score plots showed group separation, indicating that the model and rutin treatment produced distinct metabolic profiles (Fig. 4A,B). Differential feature screening identified lipid-like molecules, amino acid/peptide analogues, organic acids, carbohydrates and steroids as major changed classes (Fig. 4C,D). Pathway enrichment further indicated that alanine/aspartate/glutamate metabolism and related energy-metabolic pathways contributed to the rutin-responsive profile (Fig. 4E,F).

## 8. 图注写作规则

Each figure legend must define every panel.

Minimum requirements:

- Start with the figure's main message.
- Explain A, B, C, D, etc. in order.
- Define abbreviations.
- Include treatment concentration, timing, sample type, or model condition when relevant.
- Include statistical method, sample size, and significance notation when available.
- Do not use "same as above" unless the journal style permits it.

Useful caption skeleton:

```text
Fig. X. Main message of the figure. (A) ... (B) ... (C) ... Data are shown as mean ± SEM. Statistical significance was assessed by [test]. *P < 0.05, **P < 0.01, ***P < 0.001 versus [group]; #P < 0.05 versus [group]. Abbreviations: ...
```

If statistics are not available, write `statistical details to be confirmed` in the working draft rather than inventing them.

## 9. 材料与方法写作规则

Materials and Methods must be a formal methods section, not a single paragraph.

Common subsections:

1. Chemicals and reagents
2. Zebrafish husbandry and ethics
3. AD-like model establishment and treatment
4. Behavioral assays
5. Biochemical assays
6. Fluorescence labeling and in vivo imaging
7. AFADESI-MSI sample preparation and imaging
8. Transcriptomic analysis
9. Network pharmacology
10. Untargeted metabolomics
11. Targeted metabolomics
12. Targeted lipidomics
13. Spatial metabolomics data processing
14. Statistical analysis

The Methods section should preserve details such as:

- Model reagent and treatment time.
- Compound dose and unit.
- Animal stage and strain.
- Ethics approval number.
- Instrument manufacturer and model.
- Chromatographic column and mobile phases.
- Ion mode and acquisition mode.
- Standard calibration range.
- Internal standards.
- Software and thresholds.

Example targeted lipidomics detail:

> Targeted lipid analysis was performed using a UHPLC ExionLC AC system coupled to a QTRAP 6500+ triple quadrupole mass spectrometer. Quantification was conducted in multiple reaction monitoring (MRM) mode. Calibration standards covered 1-2000 ng/mL, including 2000, 1000, 500, 250, 125, 100, 62.5, 50, 25, 12.5, 10, 5, 2.5 and 1 ng/mL.

## 10. 讨论写作规则

A strong Discussion is not a short restatement of Results. It interprets the evidence hierarchy and explains why the study matters.

Recommended structure:

1. **Main integrated finding**: state the mechanism at the highest supported level.
2. **Model interpretation**: explain what the disease model captures and why it matters.
3. **Exposure/distribution**: discuss why tissue distribution strengthens pharmacodynamic interpretation.
4. **Primary mechanism branch**: discuss the most consistently supported pathway, such as amino acid-neurotransmitter metabolism.
5. **Complementary branch**: discuss lipid, inflammatory, immune, energy, or vascular pathways.
6. **Spatial evidence**: explain how spatial metabolomics improves over homogenate omics.
7. **Computational support**: position network pharmacology or prediction results as hypothesis-organizing, not definitive proof.
8. **Limitations and future work**: state what remains associative and what causal experiments are needed.

Avoid single-pathway overclaiming. If multiple omics layers support several branches, write the mechanism as a network.

## 11. 双语写作规则

For bilingual manuscripts:

1. Write or finalize the English scientific version first.
2. Translate into Chinese faithfully, preserving:
   - Figure references
   - Numeric values
   - Units
   - Abbreviations
   - Compound names
   - Technical terms
   - Evidence hierarchy
3. Chinese should not become shorter merely because it is a translation.
4. If Chinese and English differ, document the reason.

Good bilingual work is not "English draft plus brief Chinese summary"; both versions must be manuscript-level.

## 12. 质量控制清单

Before delivery, verify:

- All expected main figures are still present.
- Figure count did not change after editing.
- Headings are in the correct order.
- Each figure is referenced in Results.
- Each panel is explained in the legend.
- Introduction has 4 developed paragraphs.
- Discussion has enough depth and includes limitations.
- Methods are split into formal subsections.
- User-supplied corrections are incorporated exactly.
- Units are consistent.
- Ethics number is correct.
- Instrument parameters and standards are included when supplied.
- No "TODO", placeholder, or invented detail remains unless clearly marked for confirmation.
- DOCX output has been rendered and visually checked when possible.

## 13. 常见返工信号

If the user says any of the following, immediately return to the evidence ledger:

- "前言太少"
- "讨论太少"
- "结果没有对应 A/B/C/D"
- "图注太简略"
- "材料与方法怎么只有一段"
- "你丢了很多关键信息"
- "按照附件的结构整理"
- "每个结果后面放图片和图注"

These are not small polishing requests. They mean the draft failed the evidence-preservation standard.

## 14. 推荐工作顺序

For future projects, follow this sequence:

1. Read all source files.
2. Extract text and figures.
3. Build the figure-panel evidence ledger.
4. Build the story line.
5. Draft English manuscript.
6. Audit omissions against the ledger.
7. Expand Results, Methods, captions, Introduction and Discussion.
8. Render and visually inspect the manuscript.
9. Produce Chinese version.
10. Render and inspect Chinese version.
11. Deliver only final files plus a concise change summary.

## 15. 最小交付说明模板

```text
已完成中英文初稿。主要工作包括：根据主图建立结果证据链，按图后跟图注的结构重排结果，扩写四段式前言，补全分层讨论，细化材料与方法，并逐项核对图注、缩写、剂量、统计和伦理信息。已渲染检查版面，未见明显重叠或缺图。
```

## 16. 工作哲学

The manuscript should feel like it was written by someone who has looked at every figure carefully. Fluency is secondary to fidelity. A smooth draft that drops experimental detail is a failed draft. A strong draft preserves the work, shows the logic, and gives the researcher a manuscript they can actually revise toward submission.

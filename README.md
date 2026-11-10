# Carnegie Learning · DSHB ’26

**UW–Madison | Data Science in Human Behavior**  
*Team research project in collaboration with Carnegie Learning*

[Research questions](#team-and-research-questions) · [Data sources](#data-sources) · [Repository workflow](#repository-workflow) · [Deliverables](#planned-deliverables) · [Data privacy](#data-access-and-privacy)

---

## Project overview

We study **student engagement and mathematics performance** using MATHstream activity and assessment records, MATHia learning history, and classroom observations. Our goal is to understand how student behavior, prior skills, and observed affect relate to learning outcomes. These patterns can inform lesson design and help Carnegie Learning recognize when students may benefit from support.

## Team and research questions

Each team member leads a research question. We collaborate on data preparation, visualization, and documentation.

| Team member | Research question | Latest progress |
| --- | --- | --- |
| **Dasey Dang** | How do incorrect responses and prior errors relate to whether an attempt is recorded as complete? | Built an attempt-level dataset, fit a **mixed-effects logistic regression**, and evaluated predictions on held-out students. |
| **Emily Huffaker** | How do observed affective states relate to APLSE Quality and MATHstream attempt scores? | Linked BROMP observations to nearby Caliper events for the same student. Analyzed **student-level APLSE Quality** and **attempt-level scores** separately. |
| **Chloe Oh** | How does reading ability relate to passing MATHstream lessons, and does that relationship vary by lesson? | Compared a model with a common reading–passing association across lessons with one that allows the association to vary by lesson. |
| **Wendy Lee** | How do video interaction patterns relate to assessment performance and disengagement? | Used **K-means clustering** to group students by pausing, rewinding, and video completion. The next step is to compare the groups on pass rates, off-task behavior, and boredom. |
| **Jingyi Zhou** | Do students show similar performance patterns across different assessment questions? | Outlined the research question in the latest project update. |

## Data sources

| Source | What it captures |
| --- | --- |
| **BROMP** | Observer-coded classroom behavior and affect, including on-task behavior, concentration, boredom, and confusion. |
| **Caliper** | Timestamped MATHstream events, including video interactions and assessment activity. |
| **Attempt** | Assessment scores, correctness, submission timestamps, and pass status. |
| **APLSE** | MATHia learning history, including time worked and student-level APLSE Quality scores. |

## Repository workflow

1. **Clone the private repository** and run analyses in the approved data environment.
2. **Open the analysis notebook** in Quarto for `.qmd` files or Jupyter for `.ipynb` files.
3. **Document each analysis** with its required Python packages, expected inputs, and instructions for running it.

## Planned deliverables

- **Cleaned analysis datasets** with documented links across BROMP, Caliper, and APLSE, maintained in the approved data environment.
- **Shared codebook** covering data collection, variable definitions, and data types.
- **Reproducible Python notebooks** covering data preparation, feature engineering, analysis, and model evaluation.
- **Final report and executive summary** with findings, recommendations, and aggregate visualizations.

## Data access and privacy

> **Private research repository.** The Carnegie Learning Data Use Agreement governs this work. Project data are for authorized, noncommercial academic research.

- **Access.** Authorized team members access the data through the designated static IP.
- **Storage.** Keep source workbooks, row-level exports, and reports containing individual records in the approved data environment.
- **Reporting.** Share results only in aggregate to protect the anonymity of students, teachers, and schools.
- **Retention.** Securely delete exported copies at project completion or upon request, as required by the agreement.

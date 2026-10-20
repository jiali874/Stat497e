# STAT 497: Statistical Learning in the Age of Generative AI — Course Materials

## Folder layout

| Folder / file | Contents |
|---|---|
| `lectures/TopicNN_Lecture_<topic>.tex` (+ `.pdf`) | Lecture slides, Beamer, SimplePlus theme (same template as `PostHocXML.tex`). Figures referenced as `../figs/topicNN_*.png`. |
| `prompts/TopicNN_Prompts_<topic>.tex` (+ `.pdf`) | Demo deck: the prompts used in class, verbatim, with what to inspect in the AI's response, the code it should produce, and the interpretation. |
| `notebooks/TopicNN_Demo_<topic>.ipynb` | Demo notebook, executed with outputs. Saves its figures to `figs/`; runs in Jupyter or Colab (`Run all`). |
| `homework/HWNN_*.ipynb` | Notebooks that a homework refers to (e.g. the audit notebooks for HW1 and HW10). |
| `figs/` | Figures produced by the demo notebooks and used in the lecture slides. |
| `Stat497e_Homework_Assignments.docx` | Student-facing: the homework system, the report template, the interaction-log codes, the rubric, HW1–HW10 and the final project. |
| `Stat497e_Instructor_Guide.docx` | Instructor-only: the measurement design for the education paper, codebook, analysis plan, research-ethics note, rubrics, audit answer keys, topic-by-topic content map. |
| `Stat497_CourseProposal.docx` | The approved course proposal (15-week outline). |
| `stat597e_aborted/` | Materials from the earlier, discarded STAT 597 design, kept for reference. |

## Rebuilding

Slides: `pdflatex` twice in the deck's folder (TeX Live with `beamertheme-simpleplus`).
Notebooks: `jupyter nbconvert --to notebook --execute --inplace notebooks/TopicNN_Demo_*.ipynb`
from the `notebooks/` folder; then move `notebooks/figs/*.png` to `figs/`.

Python packages used by the Topic 1 materials: `numpy`, `pandas`, `matplotlib`, `scikit-learn >= 1.4`.
Later topics add `torch` or `tensorflow`, `shap`, `pot` as noted in each notebook's first cell.
# Stat497e

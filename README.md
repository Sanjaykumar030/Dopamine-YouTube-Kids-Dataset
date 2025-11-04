# Dopamine-Triggering Indicators in Children's YouTube Videos
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.16755363.svg)](https://doi.org/10.5281/zenodo.16755363)

## 📄 Description
This dataset contains **500 manually annotated YouTube videos**, including both **children-targeted** and **general audience** content. Each video is labeled based on **psychological stimulation intensity**—whether the content evokes a strong attention-holding, compulsive, or high-engagement viewing experience.

Additionally, descriptive **video features** (such as dominant color and presence of frequent scene cuts) were recorded **after labeling** and are intended for use in machine learning analysis and interpretability studies.

## 🧪 Research Context
This dataset was developed as part of a research project focused on understanding **engagement dynamics and dopamine-related behavioral patterns** in digital media targeted at children.  
A corresponding academic paper will be linked here upon publication.

---

## 📊 Dataset Schema

| Column Name              | Description                                                  |
|--------------------------|--------------------------------------------------------------|
| `video_id`               | YouTube video identifier                                     |
| `channel_name`           | Channel name                                                 |
| `video_title`            | Title of the video                                           |
| `freq_cut_per_video`     | Presence of frequent scene cuts (1 = present, 0 = absent)    |
| `video_duration_sec`     | Duration of the video in seconds                             |
| `dominant_color`         | Most persistent dominant color tone                          |
| `view_count`             | Total views at time of annotation                            |
| `title_word_count`       | Number of words in the video title                           |
| `video_category`         | YouTube category label                                       |
| `is_for_kids`            | Whether the video is tagged "Made for Kids"                  |
| `date_published`         | Publication date (DD-MM-YYYY)                                |
| `key_dopamine_factor`    | Most noticeable engagement trigger (e.g., “repetitive audio”)|
| `dopamine_label`         | `1` = High psychological stimulation, `0` = Low/normal       |

---

## 🛠️ Annotation Methodology

### Step 1 — Psychological Labeling (Primary)
Annotators **first watched each video in full** and judged whether it produced a **high psychological stimulation response**, defined by:

- Strong attentional pull
- Difficulty disengaging once started
- Perceived sensory or emotional intensity

This judgment generated the `dopamine_label`:

dopamine_label = 1 → High psychological stimulation
dopamine_label = 0 → Normal or low stimulation


**Labeling was based on psychological experience.  
No visual feature counts were referenced during labeling.**

### Step 2 — Feature Annotation (Secondary)
After the dopamine label was assigned, annotators **recorded observable video features**, such as:

- Presence of frequent scene cuts
- Dominant color tone
- Primary engagement trigger style

This ensures a clean separation:

Psychological Experience → Label
Visual & Content Properties → Features


This allows machine learning models to **learn relationships rather than replicate labeling logic**.

---

## 👥 Annotation Contributors
- **Sanjay Kumar Sakamuri Kamalakar** — Dataset design, primary annotation, feature recording  
- **Jivanthikaa KK** — Co-annotation and curation

Ambiguous labeling cases were discussed collaboratively to maintain consistency.

---

## ⚖️ Dataset Class Balance

| Label / Attribute | Count |
|------------------|-------|
| Dopamine = 1     | 250   |
| Dopamine = 0     | 250   |
| For Kids = Yes   | 250   |
| For Kids = No    | 250   |

Balanced structure ensures fair evaluation in ML experiments.

---

## ⚠️ Notes and Limitations
- Stimulation labels represent **subjective perception**, not clinical dopamine measurement.
- View counts and video context may change over time.
- Intended for **research and experimentation**, not medical or diagnostic use.

---

## 📜 License
This dataset is released under the **Creative Commons Attribution 4.0 (CC BY 4.0)** license.

You may **share, adapt, and build upon** the dataset — with attribution.

---

## 📣 Citation
**Please cite using the DOI at the top of this page.**

---

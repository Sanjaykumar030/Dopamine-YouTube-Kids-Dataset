# Dopamine-Triggering Indicators in Children's YouTube Videos

## 📄 Description
This dataset contains **500 manually annotated records** of dopamine-inducing features from **YouTube videos targeted at children**, alongside a control set of **non-children content**. It was curated to support **comparative behavioral analysis** between child-specific media and general YouTube content.

## 🧪 Research Context

This dataset was created as part of a dopamine-based research project using machine learning techniques, focusing on behavioral triggers in children's video content. The associated academic paper is under preparation and will be linked here upon publication (planned submission to arXiv).

## 📊 Dataset Schema

| Column Name              | Description                                                  |
|--------------------------|--------------------------------------------------------------|
| `video_id`               | YouTube video identifier                                     |
| `channel_name`           | Channel name                                                 |
| `video_title`            | Title of the video                                           |
| `freq_cut_per_video`     | Binary flag for frequent cuts (1 if present, 0 if absent)    |
| `video_duration_sec`     | Duration of the video in seconds                             |
| `dominant_color`         | Dominant frame color (categorical)                           |
| `view_count`             | Total number of views                                        |
| `title_word_count`       | Number of words in the video title                           |
| `video_category`         | YouTube category label                                       |
| `is_for_kids`            | Boolean indicating child-targeted content                    |
| `date_published`         | Publication date (DD-MM-YYYY)                                |
| `key_dopamine_factor`    | Dominant dopamine feature (e.g., “jingles”, “flashing”)      |
| `dopamine_label`         | `1` if dopamine-triggering, else `0`                         |

> 🧠 This dataset contains **exactly 500 records** and **13 well-defined features**, curated explicitly for **machine learning training and behavioral analysis**.

---

## 🎯 Use Cases

- Behavioral machine learning modeling  
- Media and content moderation research  
- Child psychology and media studies  
- Interpretability and SHAP-based model analysis  

---

## 🛠️ Annotation Methodology

- **video_id**: Extracted from the unique YouTube video URL.
- **channel_name**: As listed on YouTube.
- **video_title**: Cleaned version of the video title (special characters removed when necessary).
- **freq_cut_per_video**: Manually annotated presence of frequent scene cuts; only binary observation noted.
- **video_duration_sec**: Converted to seconds for standardization.
- **dominant_color**: Most persistent color observed in the video’s frames.
- **view_count**: Snapshot of views at the time of annotation.
- **title_word_count**: Counted after cleaning punctuation/symbols.
- **video_category**: Assigned based on YouTube classification and contextual judgment.
- **is_for_kids**: Based on YouTube’s “Made for Kids” tag.
- **date_published**: As listed by the video creator, formatted as DD-MM-YYYY.
- **key_dopamine_factor**: Major trigger features like **familiarity**, **animation**, or **music repetition**; "No Dominant Factor" if none detected.
- **dopamine_label**: Binary label manually assigned based on holistic feature evaluation. It reflects annotation judgment and is **not a definitive neuropsychological metric**.

---

## ⚠️ Caution

- All annotations are **manual** and may contain **subjective bias or human error**.
- **View counts** represent values at the time of annotation and may not be current.
- The dataset is designed for **experimental research only**, not clinical applications.

---

## 📜 License

This dataset is licensed under the **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)** license.

You are free to:

- **Share** — copy and redistribute the material in any medium or format  
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:

- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

## 👥 Contributors

- **Sanjay Kumar Sakamuri Kamalakar** (Lead Creator, Dataset Design, Feature Engineering)  
  GitHub: [@Sanjaykumar030](https://github.com/Sanjaykumar030)  
  ORCID: [0009-0009-1021-2297](https://orcid.org/0009-0009-1021-2297)

- **Jivanthikaa KK** (Co-author, Dataset Annotation and Curation)  
  ORCID: [0009-0009-7939-3524](https://orcid.org/0009-0009-7939-3524)


## 📣 Citation

This dataset will be assigned a DOI upon publication via [Zenodo](https://zenodo.org).  
Please cite it using the official Zenodo citation once available.

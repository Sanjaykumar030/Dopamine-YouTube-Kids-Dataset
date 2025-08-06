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
| `freq_cut_per_video`     | Count of fast cuts                                           |
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

This dataset is released under the **MIT License**.

> Permission is hereby granted, free of charge, to any person obtaining a copy  
> of this dataset and associated documentation files (the "Dataset"), to deal  
> in the Dataset without restriction, including without limitation the rights  
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell  
> copies of the Dataset, and to permit persons to whom the Dataset is  
> furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all  
> copies or substantial portions of the Dataset.

**License File:** [`LICENSE`](./LICENSE)

[MIT License — Full Text](https://opensource.org/licenses/MIT)

## 📣 Citation

This dataset will be assigned a DOI upon publication via [Zenodo](https://zenodo.org).  
Please cite it using the official Zenodo citation once available.

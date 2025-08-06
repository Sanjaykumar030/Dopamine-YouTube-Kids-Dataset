# Dopamine-Triggering Indicators in Children's YouTube Videos
## Description
This dataset contains 500 manually annotated records of dopamine-inducing features from YouTube videos targeted at children, alongside a control set of non-children content. It was curated to enable comparative analysis of behavioral triggers in children's media versus general content.
##  Dataset Schema
| Column Name             | Description                                                  |
|-------------------------|--------------------------------------------------------------|
| `video_id`              | YouTube video identifier                                     |
| `channel_name`          | Channel name                                                 |
| `video_title`           | Title of the video                                           |
| `freq_cut_per_video`    | Count of fast cuts                                           |
| `video_duration_sec`    | Duration of the video in seconds                             |
| `dominant_color`        | Dominant frame color (categorical)                           |
| `view_count`            | Total number of views                                        |
| `title_word_count`      | Number of words in the video title                           |
| `video_category`        | YouTube category label                                       |
| `is_for_kids`           | Boolean indicating child-targeted content                    |
| `date_published`        |  Publication date                                     |
| `key_dopamine_factor`   | Dominant dopamine feature (e.g., “jingles”, “flashing”)      |
| `dopamine_label`        | `1` if dopamine-triggering, else `0`                         |

This dataset exactly contains 500 records and 13 columns which was explicitly made for Machine Learning model training 
## Can be used for

- Behavioral ML modelling
- Content moderation research
- child psychology and media studies

## Methodology of Annotation
- video_id: Taken from the directory of the youtube video's unique identifier.
- channel_name: As shown in the Youtube
- video_title: The main title of the video without considering any special characters in it and sometimes the own channel name.
- fre_cut_per_video: Due to manual annotation the only whether the presence of the freq cuts are observed instead of calculating it. Frequent cuts are carefully observed and annotated.
- video_duration_sec: Actualy video duration was converted into seconds as a standard of annotation.
- dominant_color: Based on the most dominating color on the video for a significant amount of time is manually annotated.
- view_count: Views reached till the annotated period
- title_word_count: Number of words involved in vidoe's title is taken
- video_category: Based on the content and reach the category is selected
- is_for_kids: Using Youtube's predefined categorization of "video made for kids"
- date_published: The date published by the content creator in DD-MM-YYYY format
- key_dopamine_factor: Based on video's popularity, content, intention and possible triggering factors present, the video is categorised into special factors like "Familiarity" (eg.MrBeast), "No Dominant Factor" if the video is not meant for any specific dopamine triggers.
- dopamine_label: Based on the all the other features and manual annotation. The final dopamine label is annated and it doesn't gurantee a definitive conclusion
  




## Caution
- Since, the whole dataset is manually annotated there is a possiblity for human error.
- Dataset involves views of each video and it is subjected to annotated date only.



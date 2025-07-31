# Data Dictionary

This document provides descriptions for the columns in the datasets used for the **LEGO Sets History Analysis** project.

## lego_sets.csv

| Column Name | Description |
|----------------|--------------------------------------------------------|
| `set_num` | Unique identifier for each LEGO set. Missing values may indicate duplicates or invalid entries. |
| `name` | Name of the LEGO set. |
| `year` | Year the set was released. |
| `num_parts` | Number of pieces in the set. Not central to current analysis; nulls are acceptable. |
| `theme_name` | Sub-theme name of the LEGO set. |
| `parent_theme` | Name of the parent theme. Matches the `name` column in `parent_themes.csv`. |

------------------------------------------------------------------------

## parent_themes.csv

| Column Name | Description |
|----------------|--------------------------------------------------------|
| `id` | Unique identifier for each parent theme. |
| `name` | Name of the parent theme. Used in merging with `lego_sets.csv`. |
| `is_licensed` | Boolean value (`True`/`False`) indicating whether the theme is licensed. |

------------------------------------------------------------------------
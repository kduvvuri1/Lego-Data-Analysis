
# LEGO Sets Analysis

## Introduction

This project explores the history and data of LEGO sets, focusing on the introduction and impact of licensed themes such as Star Wars, Super Heroes, and Harry Potter. The project examines how LEGO overcame financial difficulties in the late 1990s and thrived due to the success of its licensed sets.

### Objectives
- Analyze the history of LEGO sets to identify trends and insights.
- Answer key business questions about licensed LEGO themes.

## Datasets

### 1. `lego_sets.csv`
- **set_num**: Unique identifier for each LEGO set.
- **set_name**: The name of the LEGO set.
- **year**: Release year of the LEGO set.
- **num_parts**: Number of parts in the LEGO set.
- **theme_name**: Sub-theme name of the LEGO set.
- **parent_theme**: Parent theme of the LEGO set, linked to `parent_themes.csv`.

### 2. `parent_themes.csv`
- **id**: Unique identifier for each parent theme.
- **name**: Name of the parent theme.
- **is_licensed**: Boolean indicating whether the theme is licensed.

## Business Questions
1. What percentage of all licensed sets ever released were Star Wars themed?
2. How have licensed themes influenced LEGO's overall success?

## Methodology
- **Tools Used**: Python, pandas library for data analysis.
- **Steps**:
  1. Load and explore the datasets.
  2. Perform data cleaning and preprocessing.
  3. Analyze the data to answer the business questions.
  4. Visualize the results where applicable.

## Sample Code
```python
# Load datasets
import pandas as pd

df = pd.read_csv('https://raw.githubusercontent.com/KeithGalli/lego-analysis/master/datasets/lego_sets.csv')
theme = pd.read_csv('https://raw.githubusercontent.com/KeithGalli/lego-analysis/master/datasets/parent_themes.csv')

# Display the first few rows of the parent themes dataset
theme.head()
```

## Conclusion
This project sheds light on the impact of licensed LEGO sets on the company's success. By analyzing trends in the data, we gain a better understanding of how strategic decisions, such as partnerships, have shaped LEGO's trajectory.

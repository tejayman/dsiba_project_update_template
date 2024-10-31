# Project Update Report: Code and Structure

## Group Name: Group X

### Authors: Author 1, Author 2

This README file provides a general structure of the project directory to help navigate and reproduce the results effectively.

### Project Structure

The project is organized into the following main directories:

```
.
├── data          : Contains processed and cleaned data files used in analysis.
│   ├── raw       : Contains the original, unprocessed data files as you have retrieved them.
│   └── processed : Contains the cleaned and processed data files.
├── report        : Stores all files related to the project update report.
│   ├── sections  : Contains separate `.qmd` files for each report section.
│   └── report.qmd: Main Quarto file that combines all sections into a full report.
└── src           : Source code directory with all R scripts used for data cleaning, analysis, and visualization.
```

### Directory Details

- **`data/`**: Processed versions of the raw data, ready for analysis.
- **`data/raw/`**: Original datasets and any raw files collected for the project. **Do not modify these files**. This is especially important for reproducibility purposes.
- **`data/processed/`**: Processed versions of the data should be saved in `data/processed`.
- **`report/`**: Contains the Quarto files used to generate the report, with sections organized to allow for modular writing and updating. `report.qmd` is the main Quarto file that combines all sections into a single HTML or PDF report.
- **`src/`**: Contains R scripts organized by function, e.g., data cleaning, EDA (Exploratory Data Analysis), and statistical analysis. Each script should have clear comments explaining its role.

### Good Practices

- **Set a Seed**: Always set a random seed in your R scripts to ensure reproducible results.
- **Version Control**: Use `git` and `GitHub` for version control to keep track of changes in your code and facilitate collaboration within the group. You can also use a file called `.gitignore` to exclude certain files from version control (i.e., being pushed to GitHub). The `.gitignore` file is set up to exclude `.Rhistory`, `.RData`, and large datasets files (even entire directories) that go over GitHub's file size limit.

---

### Reproducibility

To reproduce this project:

1. Clone the repository.
2. Run each script in `src` as needed, following any instructions or comments within each script.
3. Compile the final report by knitting `report/report.qmd` into HTML or PDF format.

With this structure and setup, your project is organized for clear navigation and efficient collaboration.

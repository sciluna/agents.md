# Coding Agent Notes

## Coding Preferences
- Prefer R code for analysis scripts
- R scripts in this repo should not include a shebang line or calls to `suppressPackageStartupMessages`.
- Prefer snake_case identifiers for variables, functions, and files.
- Add concise comments to delineate major sections (for example, data loading, preprocessing, plotting) and document helper functions.
- When generating plots, ensure exported images use explicit white backgrounds.
- Analysis script names should be clear file names to suggest purpose (don't rename existing scripts); there should be comments that provides clear purpose for the script
- Use `roxygen` to provide documentation for any functions created
- Attempt to use `ggplot` for R plots; generate both png and pdf for images using ggsave
- Use `ggrepel` to label highlight points in differential-expression volcano plots with the gene names represented.
- Assume `tidyverse` packages are installed 
- Use `ComplexHeatmap` for heatmaps
- Prefer `ggvenn` for set/overlap visualizations

## File Structure
- Data (e.g., input -omics data) in /data also data annotations and secondary inputs puts like gene sets
- Output (/output) are outputs of analyses such as tables or plots with sub-directories for particular analyses
- Scripts (/scripts) analysis scripts
- Write scripts that avoid hard-coded file paths; assume users set the project directory as the working directory with setwd()

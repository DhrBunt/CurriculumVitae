## My pagedown rendered CV

This repo contains the source-code and results of my CV built with the [pagedown package](https://pagedown.rbind.io) and a modified version of the 'resume' template. 

The main files are:

- `Resume.Marco.Bunt.Rmd`: my cv, nerd style cv.
- `Resume.Marco.Bunt.html`: The final output of the cv.
- `positions.csv`: A csv with columns encoding the various fields needed for a position entry in the CV. A column `section` is also available so different sections know which rows to use.
- `css/`: Directory containing the custom CSS files used to tweak the default 'resume' format from pagedown. 

## Want to use this to build your own CV/resume? 

1. Fork, clone, download the zip of this repo to your machine with RStudio.
2. Go through and personalize the supplementary text in the Rmd you desire (`index.Rmd` for CV, `resume.Rmd` for resume).
3. Using your spreadsheet editor of choice, replace the rows of `positions.csv` with your positions.
3. Print each unique `section` (as encoded in the `section` column of `positions.csv`) in your `.Rmd` with the command `position_data %>% print_section('education')`.

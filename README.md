# Generating a Stat Block for the Calculus Baseline Assessment

This repository allows you to have your calculus readiness gauged
based on your performance on the calculus baseline assessment (CBA).
In order to properly use this repository, it is recommended that you
follow the steps as outlined below:

1. Read the `cba_files/cba_assessment.pdf`.
2. Complete the assessment by drafting two files: `cba_example/cba_mc_submission.txt` and `cba_example/cba_text_submission.txt`.
3. The file `cba_example/cba_mc_submission.txt` should be written as a string of twenty characters, each one sequentially describing the option you select for a CBA question.
4. The file `cba_example/cba_text_submission.txt` should be written with `Q- ` at the start of each question. Be sure to have a linebreak before the start of each new question. Your text responses should describe your solution process for the question in plain language while relying as little as possible on mathematical formula.
5. Once your files are completed, access `cba_plot_generator.ipynb` in order to automatically grade your CBA, have it assigned qualitative codes, and then have those data values returned to you as a spider plot.

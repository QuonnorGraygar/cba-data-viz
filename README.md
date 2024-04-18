# Generating a Stat Block for the Calculus Baseline Assessment

In the preprint *Understanding Dimensions of Student Readiness from a Calculus Baseline Assessment through Semi-Automatic Text Analysis and Clustering*, we introduce a diagnostic tool that is intended to gauge the level of preparedness for students who are beginning their first undergraduate calculus course. In particular, we start with a multiple-choice format inspired by the Precalculus Concept Assessment (Carlson et al., 2010) and the Calculus Concept Readiness instrument (Carlson et al, 2015), and pair each question with an "explain your reasoning" text prompt. The results gathered by this tool allow for the formation of a multi-dimensional view of student readiness through qualitative coding of the text responses. The codes are categorized into a taxonomy that gauge and observe various student behaviours. Manually coded responses are used as a training set for the fitting of a gradient boosting machine model, which automatically codes additional responses at a fixed cost. Compared against a manual coder's assessment of a held-out validation, the automatic coder averaged over 80% matching accuracy. Using these qualitative codes as vector dimensions, $k$-clustering of student demographic allows for the visualization of theoretical student archetypes that exist within a large first-year undergraduate math class. These visualizations are made possible using spider plots.

This repository allows you to have your calculus readiness gauged based on your performance on the calculus baseline assessment (CBA). Note that the machine learning models used to classify your text responses were trained on a dataset consisting of approximately 500 responses from a first year undergraduate course held during the 2022-2023 academic year at a large reserach-intensive public Canadian Univeristy. As such, the model may not be well-tuned to responses outside of this specific context. 

The raw text data used to build these models is unavailable for public use. Due to the ethics guidelines agreed upon to prior to data collection, we are unable to share raw data files to anyone outside of the research team. Any available data that is able to be shared is already on this GitHub repository.

If you use any of this repository as part of a published work, we ask that you cite us accordingly. If you are interested in this project and would like to learn more, please see the [slide deck](https://github.com/QuonnorGraygar/cba-data-viz/blob/main/cba_example/cba_presentation.pdf) from a recent presentation and/or contact our research team:
- Connor Gregor, Postdoctoral Fellow, Department of Mathematics and Statistics, McMaster University (gregoc9@mcmaster.ca)
- Caroline Junkins, Assistant Professor, Department of Mathematics and Statistics, McMaster University (junkinc@mcmaster.ca)
- Lindsey Daniels, Assistant Professor of Teaching, Department of Mathematics, University of British Columbia (ldaniels@math.ubc.ca)

&nbsp;
&nbsp;

In order to properly use this repository, it is recommended that you follow the steps as outlined below:

1. Read the `cba_files/cba_assessment.pdf`.
2. Complete the assessment by drafting two files: `cba_example/cba_mc_submission.txt` and `cba_example/cba_text_submission.txt`.
3. The file `cba_example/cba_mc_submission.txt` should be written as a string of twenty characters, each one sequentially describing the option you select for a CBA question.
4. The file `cba_example/cba_text_submission.txt` should be written with `Q- ` at the start of each question. Be sure to have a linebreak before the start of each new question. Your text responses should describe your solution process for the question in plain language while relying as little as possible on mathematical formula.
5. Once your files are completed, access `cba_plot_generator.ipynb` in order to automatically grade your CBA, have it assigned qualitative codes, and then have those data values returned to you as a spider plot.

&nbsp;
&nbsp;

References:
- Carlson, M., Oehrtman, M., & Engelke, N. (2010). The precalculus concept assessment: A
tool for assessing students’ reasoning abilities and understandings. *Cognition and Instruction,
28(2),* 113-145.
- Carlson, M.P., Madison, B. & West, R.D. A Study of Students’ Readiness to Learn Calculus.
*Int. J. Res. Undergrad. Math. Ed.* 1, 209–233 (2015).
- Carlson, M. O. Madison B. & West. R. D. The Calculus Concept Readiness (CCR) Instrument:
Assessing Student Readiness for Calculus. *arXiv preprint arXiv:1010.2719* (2010).

&nbsp;

This work was overseen by the McMaster Review Ethics Board (MREB\#: 6043) and University of British Columbia's Behavioural research ethics board (UBC BREB\#: H22-02247) who carefully 
reviewed our study and ensured the protocols are consistent with research ethics. 




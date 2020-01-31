
# Identifying strong predictors of breast cancer recurrence

Group Members: Haoyu(Clara) Su, Fanli Zhou, Ke Xin(Margaret) Zhao

We explored to use a logistic regression model to identify strong
predictors of breast cancer recurrence. Based on the feature weights
assigned in the model, we found that degrees of malignancy are very
strong predictors of breast cancer recurrence. The other two predictors,
including being in the age 60-69 group and having cancer in the right-up
of the breast quadrants, are also among the top five features with the
highest absolute weight values. Our model didn’t perform well on unseen
data, with a fair accuracy score of 0.73 and a low recall score of 0.25.
The low recall score is likely due to the data imbalance problem noticed
in the training data set. If time permits, we would like to explore some
advanced methods to handle the imbalanced data situation and try some
advanced feature selection methods to build a better model.

The breast cancer data set was obtained from the UCI Machine Learning
Repository (Dua and Graff 2017) and can be found
[here](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer). The data
set looks at the recurrence and non-recurrence of breast cancer based on
9 features, including groups of age, menopause time, tumor size, ranges
of the number of axillary lymph nodes, presence of node in cap, degree
of malignancy, breast type, breast quadrant, and whether the patient
used radiation therapy. The data set contains 286 instances with missing
values.

## Report

The final report can be found
[here](https://github.com/UBC-MDS/DSCI_522_Group_301/blob/master/doc/report.md)

## Usage

To replicate the analysis, clone this GitHub repository, install the
[dependencies](#dependencies) listed below, and run the following
commands at the command line/terminal from the root directory of this
project:

    make all

To reset the repo to a clean state, with no intermediate or results
files, run the following command at the command line/terminal from the
root directory of this project:

    make clean

## Dependencies

  - Python 3.7.4 and Python packages:
      - pandas==0.25.2
      - numpy==1.17.2
      - altair==3.3.0
      - sklearn==0.22
      - docopt==0.6.2
  - R 3.6.1 and R packages:
      - knitr==1.27.2
      - tidyverse==1.3.0
      - ggridges==0.5.1
      - cowplot==1.0.0

# References

<div id="refs" class="references">

<div id="ref-Dua2019">

Dua, Dheeru, and Casey Graff. 2017. “UCI Machine Learning Repository.”
University of California, Irvine, School of Information; Computer
Sciences. This breast cancer domain was obtained from the University
Medical Centre, Institute of Oncology, Ljubljana, Yugoslavia. Thanks go
to M. Zwitter; M. Soklic for providing the data.
<http://archive.ics.uci.edu/ml>.

</div>

</div>

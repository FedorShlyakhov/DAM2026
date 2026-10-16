# DAM2026

# Exam project guidelines

As mentioned in the [course overview](https://github.com/FedorShlyakhov/DAM2026/blob/main/01-intro/DAM-2026-course-overview.pdf),
the exam project is about participating in a competition.
**Please write me to e-mail to confirm your choice**.

There are 3 main checkpoints for the project:
|Checkpoint|Deadline|
|--|--|
|Topic choice| October 16 |
|Intermediate status report|November 13|
|Project defense| December 4 & 11|

- Missing dedline for stage 1, 2 will result in -1 point (for each stage) for the project.
- Missing the project defense (stage 3) will result in 0 for the whole project.
- All members of a group need to attend the final defense.

The topic choice needs to be approved, so make sure you leave some time before the deadline for possible refinements.

The intermediate status report should cover at least 50% of the work that will be done by the project defense.
This intermediate report should consist of a GitHub repository with your code, where your
**Continuous progress should be clearly seen** (if you're participating in a competition within a team,
**Contributions from all the members should be seen explicitly, via commits**).
Also, a brief supporting document should be provided (e.g. text or slides with comments) describing what
you have done and what you are planning to do by the end of the project.
The report will be graded in a binary form (passed/failed).

The project defense will be organized in a form of a public presentation of roughly 15-20 minutes per person (group).
A successfully passed intermediate status report is necessary to be admitted for the project defense.
You can find some guidelines below for the project.


## Competition

The main goal of a competition exam project is for you to demonstrate your skills in solving a real-world data analytics and machine learning problem. When choosing a competition, please avoid the ones tagged with the `Getting Started` or `Playground`
tags. Ideally, it should be an ongoing (or a finished competition with late submission allowed)
from the [`Monetary` category](https://www.kaggle.com/competitions?prestigeFilter=money). This competition may be taken in
a team of up to 3 members. If so, the roles of all the members should be clearly stated and significant.
**Contributions from all the members should be seen explicitly, via commits in your project repository**
All members should participate in the project defense (public presentation).
A single competition may only be approved to at most 9 people (e.g. 9 individuals, 3 teams of 3, or anything in between).

You can consult the existing solutions, shared kernels, etc. but blind re-use of such materials is prohibited.
If you are basing (a part of) your solution on someone else’s work, be sure to make a proper reference to
that work, and also to have a sizable personal contribution on top of that.

## Intermediate status report (November 13): requirements

The report is graded pass/failed. It passes if everything below is in place.

### Repository

- A GitHub repository with a README: the competition (with a link), the target and the evaluation metric, the team members and their roles.
- In a team, every member has commits that correspond to their role.

### Work done (at least 50% of the project)

- Data loading and a description of the data: number of rows and columns, feature types, what each feature means.
- Exploratory data analysis: the distribution of the target, distributions of the main features (histograms for numeric features, bar charts for categorical ones) with short comments, and relations between the main features and the target.
- Missing values and anomalies: where they are, how many, and how you handle them (drop, fill or flag), with a reason for the choice.
- Preprocessing: encoding of categorical features, scaling where the model needs it.
- A validation scheme (hold-out or cross-validation) with the competition metric computed on it.
- A baseline: a trivial prediction (a constant, the most frequent class or a simple rule) and at least one trained model, both scored on validation.
- At least one successful submission on Kaggle.

### Supporting document (1–2 pages of text or 3–5 slides)

- What has been done, including the key EDA findings and the current scores (validation and Kaggle).
- What is planned until the defense, and who will do what.

## Final grading (10 points)

### 1. Problem and data (2 points)

- **0.5:** the task, the target and the metric are explained in plain words, including what the metric rewards.
- **1:** EDA. Distributions of the target and the features are shown and interpreted, relations with the target are explored, and the findings are stated, not just plotted.
- **0.5:** missing values, outliers and other data problems are identified.

### 2. Preprocessing and features (2 points)

- **0.5:** missing values are handled and the choice is justified.
- **0.5:** categorical encoding and scaling are appropriate for the models used.
- **1:** feature engineering and selection. At least two new features are built (or irrelevant ones are removed), and their effect on the validation score is checked.

### 3. Models (2.5 points)

- **0.5:** a baseline (trivial prediction) to compare against.
- **1:** at least three different types of models, for example a linear model, a random forest and gradient boosting.
- **1:** hyperparameters of at least one model are tuned on validation (grid search, random search or similar), and the tuning is described.

### 4. Evaluation and model choice (1.5 points)

- **0.5:** a validation scheme using the competition metric, without leakage (preprocessing is fitted on the training part only).
- **0.5:** a table comparing all models on the same validation.
- **0.5:** the final model is chosen for a stated reason. Validation and leaderboard scores are compared and the difference is discussed.

### 5. Presentation (2 points)

- **0.5:** clear structure: problem, data, what was done, results, conclusions.
- **0.5:** readable slides: plots with labeled axes and readable fonts, results in tables, no screenshots of code and no walls of text.
- **0.5:** the talk fits into 15–20 minutes, and in a team every member presents their own part.
- **0.5:** answers to questions show that the speakers understand and can justify their choices.

### Notes

- Code taken from public notebooks without a reference is not graded. With a reference, only your own contribution on top of it is graded.
- Presenting is a blocking activity, which means that your team have to present to get points for 1-4 Sections!

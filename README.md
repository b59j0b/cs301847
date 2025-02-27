java cFinal project
Computational Cognitive Science: Winter Term 2024/2025
December 18, 2024
Project Deadline: 03.03.2025
Task Instructions
• Choose one of two available data sets (see last page for descriptions). Each dataset consists of multiple
participants performing on either 1) delay discounting task or 2) probability discounting task. Your task
is to infer, evaluate, and compare (at least) three distinct bi-modal probabilistic models.
The two modalities to consider are 1) choice and 2) reaction times observed during each trial of the
experiment.
All three of your models should use the same choice modeling (e.g., one discussed in class), but distinct
reaction time (RT) modeling. For reaction time, please come up with psychologically reasonable process
models; check current scientific literature to develop your ideas.
• Each dataset consists of two experimental runs: run A and run B. Your models are to be inferred on run
A while evaluated and compared on run B.
• Assess the performance of your models, evaluate their ability to predict both the participants’ choices and
their reaction times. Choose carefully and use performance metrics discussed in class to measure model
quality. Present your evaluation results using statistical summaries and graphical visualizations. Make
sure that you separately analyze and report findings for the ’reward’ and ’loss’ experimental conditions
(as described in the dataset details).
• After the analysis and comparison, finalize and recommend one (or more) model(s) with a clear argument
why it is the best choice.
Formatting Instructions
• Hand in a written report and all the code used to infer and evaluate models.
• Code: Submit in form of jupyter notebook.
• Written report: Max 5 PDF pages in total, using format in macros FP. Title page (tile, names, and
summary), figures, and tables do not count into the page count.
• Handing in in groups: Max. 3 students per group. Clearly assign credit to students! Recommendation:
Each student comes up with an own model, and implements the entire pipeline from model inference to
model evaluation.
• Formatting of written report: See individual section for instructions.
Summary Add word summary of your project (max. 250 words).
Note: Please mention in your submission weather you need a full grading or just a qualifying decision on
pass / fail. Your projects will be graded accordingly.
1
Project structure: Ideal project structure has been provided below
1 INTRODUCTION
0.5 to 1 page
2 METHODS
1 to 2 pages
2.1 Data
Describe the data you used.
2.2 Behavioral Models
Use statistical and mathematical notation to describe your models, see exercises for reference.
2代 写data、MATLAB
代做程序编程语言.3 Data Analysis
Analyze your data and make inferences about the models, their prediction accuracy etc. Make graphical repre sentations to explain your inferences.
3 RESULTS
1 to 2 pages.
3.1 Prediction Error Assessment
3.2 Additional Results
4 DISCUSSION
0.5 to 1 page
2
DATASET DESCRIPTIONS
Dataset 1: Probability Discounting Data Set
In the uploaded zip folder ”PD data.zip”, you will find 49 MATLAB data files obtained from 49 participants
performing on a probability discounting task experiment. In each trial of this experiment, a participant has to
choose between two options: a smaller certain reward vs. a larger uncertain reward.
In each file, you will find three data structures (that you can load in via pandas https://pandas.pydata.
org/):
• data train: matrix that contains trials of an initial experiment
• data test: matrix that contains trials of a successive experiment
• data labels: array of strings, describing each column in the former two data matrices
In the data matrices, the rows specify the settings of each experimental trial (starting from trial 1 to trial N).
The 8 columns contain the following information
1. Reward magnitude for the certain choice rcert
2. Reward magnitude for the uncertain choice runcert
3. Event outcome probability
4. Choice (1=certain, 2=uncertain, 0=missing)
5. p cert (experimental conditions)
6. Condition (1=reward discounting, 2=loss discounting)
7. Reaction time
8. Odds
Dataset 2: Delay Discounting Data Set
In the uploaded zip folder ”DD data.zip”„ you will find 99 MATLAB data files obtained from 99 participants
performing on a delay discounting task experiment (with two samples from two experiments with slightly dif ferent experimental setups). In each trial of this experiment, a participant has to choose between two options: a
smaller immediate reward vs. a larger delayed reward.
In each file, you will find three data structures (that you can load in via pandas https://pandas.pydata.
org/):
• data train: matrix that contains trials of an initial experiment
• data test: matrix that contains trials of a successive experiment
• data labels: array of strings, describing each column in the former two data matrices
In the data matrices, the rows specify the settings of each experimental trial (starting from trial 1 to trial N).
The 8 columns contain the following information
1. Reward magnitude for the immediate choice rimm
2. Reward magnitude for the delayed choice rdel
3. Delay
4. Choice (1=immediate, 2=delayed, 0=missing)
5. p imm (experimental conditions)
6. Condition (1=reward discounting, 2=loss discounting)
7. Reaction time
3

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com

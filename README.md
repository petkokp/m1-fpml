# Foundational Principles of Machine Learning

Gitlab for the course Foundational Principles of Machine Learning (FPML or T2A) in the CS Masters (M1 year), in the track *Artificial Intelligence* of the Paris Saclay University

Lectures in room B108 at 9:00

TP in rooms E203 and E204 at ~10:45

The e-campus address is (for the quizz):

https://ecampus.paris-saclay.fr/course/view.php?id=154572#section-7

# REMOTE CLASS - Nov 22 - class in remote only !!

Dear students
(I expect all students are now in the list - maths&AI students, please check you are all registered ?),

tomorrow the class of FPML will be held online.
The lecture will occur at 9:00, and the tutorial around 10:45
A quiz (about session 1 = lecture1 + tutorial1) will be held at 12h30, to not accumulate lateness in quiz sessions.
The quiz about session 2 the quiz about session 3 will happen next week.

For the Lecture, the link is :
https://bbb.lisn.upsaclay.fr/b/fra-c7e-tmk-oeb

For the tutorials, there will be one group here:
https://bbb.lisn.upsaclay.fr/b/fra-2f5-8b7-9de

and the second group, with Nicolas, here:
https://bbb.lisn.upsaclay.fr/b/fra-p3e-mhl-27k

See you tomorrow,
Stay warm,
François Landes


# Warning: please check that you can access the quizz on ecampus !!
https://ecampus.paris-saclay.fr/course/view.php?id=154572#section-7

# If you don't have access to the quizz: email me (and tell me your @etu-upsaclay.fr address)

Uncomfortable with numpy ? Try these exercises:

https://www.machinelearningplus.com/python/101-numpy-exercises-python/

# To prepare for the exam:
- remember that you are allowed for 6 pages (3 sheets x2 sides = 6 pages) of your own personal (typically handwritten) notes.
- annals of past exams (and sometimes corrections) are available on the gitlab: 2023 and 2022 are relevant and have a corrections. 2021 is relevant but without correction. 2020 is relevant, but less than the others, and there is no formal correction, but the papers of excellent students whom basically did everything correctly, are available.

- if you feel lost with the maths, in one or several subjects:
    - The Bishop book is my main reference:https://www.microsoft.com/en-us/research/publication/pattern-recognition-machine-learning/  (free pdf !)
    - At the end of my slides (available on the gitlab), each time or almost, the last page (or previous-to-last) contains precise references (like a small range of pages from a book, or a precise web reference) that are helpful to understand that given lecture (the one presented in these slides).
    - For Algebra: Try the Bishop book, appendix C
    - For derivatives: Try the Bishop book, Appendix D
    - For probabilities (Very very basic stuff), you can try the Bishop, pages 12-20 (section 1.2 Probability Theory - the first few subsections).

- if you want an intro on lagrange multipliers: Try his appendix E




# Hint from a student from a previous year: (authentic quote)
"This class is one of the basics (with Applied Stats for instance) that really teach you what you will need later." So, spending time studying this class is a good investment for later: either you study now and do good at the exam, or you'll have to study the same stuff later in the year for the following classes.

"study regularly" -> very good idea.

# IMPORTANT: PRE-REQUISITES !

**PRE1 and PRE2 as prerequisites, and PRE4 is strongly recommended**. Note that **PRE1 and PRE2 are mandatory, i.e. you must attend them to be allowed to follow TC0/FPML**, except if you can argue that you are already very fluent in statistics (PRE1) and linear algebra (PRE2) (in that case, e-mail me).
**This class** (or an equivalent) **is a prerequisite for almost all other [AI] classes**.


# What we will do/did in class

I keep last year's notes as a guide for waht we aim to do, and attempt to update it with what we actually did this year, as the year goes:

## session 1  - GD+Linear Regression (+organizational stuff)

During the first session, we did (i give the paths to files from the gitlab):

- read together "the rules": 0-organization-rules-intro/0-organization-rules.pdf
- The main Lecture material was: 1-Regressions: lecture1-ML-vocab+LinReg.pdf (all of it)
- Still lecture material: 1-GradientDescent/Gradient Descent-demo-compute2gradients.ipynb  : I parsed it very quickly.

In tutorial, we did (may depend slightly on the group you are in):

- 1-Regressions: TD-Regressions.pdf -> we did the 1.1.1, 1.1.2, maybe the 1.1.3 (it's not very different from those before if you understand how to vectorize everything),
- in terms of notebooks, you filled the TP1.1-LinearRegression-GradientDescent.ipynb (either skipping the naive version and going directly for trick of the ones, or not), some people did also the TP1.2-LinReg-d-dimensional.ipynb (which is very similar to TP1.1)

- NOTE: sorry I did not introduce the train/test split in the Lecture, while it's mentionned in the TP (tutorials). This will be explained in depth later during the lecture.



## session 2  - Perceptron

Lecture: we covered 2-Perceptron.pdf until page 16 included.

Tutorial:
- we covered pen-and-paer exercise 2.1.1, Perceptron – classics (from TD-Classifications-subject.pdf).
- we coded a good piece of what is asked in TP2.1-Perceptron.ipynb, i.e. up to 2.1 for everyone, and a number of people also so that "it works" on MNIST, i.e completed the part "2.2 Testing on more realistic data: MNIST (restricted to 2 classes)". One needs to encode the y's in {-1,+1}. Note that the dataset is a bit too small and here we did not split in train/test/validation, we can overfit.

We did not touch TP2.2-MultiClass-Classification.ipynb


## session 3 - overfitting, regularizations

Lecture: overfitting + regularizations
- overfitting: we did it "inverted class" mode, and then normal (fast) mode.
- regularization: we covered generalties, Ridge in detail, and the Lasso, a bit.
- we did **not** do any Bayesian calculus. It'll be for next time.

Tutorial:
- Exercices 3.1 to, 3.3, i.e., explicitly: 3.1.a, 3.1.b, 3.2, then 3.3.a, 3.3.b (all this is pen and paper)
- Then question 3.3.c is actually a pointer to 3.3.c-TP-toy example Lasso.ipynb
- we did not do question 5 of 3.3.c-TP-toy example Lasso.ipynb, which is for next time



## session 4 - Maximum A Posteriori (MAP) and its link to regularization - a Multi-Class framework (OVR)


Lecture:
- MAP (Maximum A Posteriori), in general (for any statistical inference)
- Ridge Regression interpreted as a prior on weights (MAP !)
- Elastic Net, Graphical Models : 2 words
And, taking from the folder "optional material from previous or missed sessions":
- multi-class classification: complete the last bits of Lecture1/2, that we forgot to cover ! (`2-Multi-class-classification-end.pdf`)

Tutorial:
- from TD-regularizations.pdf, 3.4.a, 3.4.b Maximum A Posteriori (in general) and 3.5.b Maximum A Posteriori (for regularization) as well (the (3.5.a) was covered during the Lecture)
- (we did not have the tie for this) TP5.1-coding your own Lasso-subject.ipynb -> code it ! Here we use Objected Oriented Programming, i.e. nice lcasses in numpy, sklearn-style

## session 5 - dimensional reduction (PCA) or expansion (feature maps)

Lecture:
- PCA from scratch + what PCA is about
- feature maps (`3-2FeatureMaps.pdf`)
- catch up on multi-class classification, if not done already


Tutorial:
- feature maps: playing around
- some attacked the PCA (see 6.3-PCA-from-scratch+overfitting-correction.ipynb) first. Especially the part where you re-code PCA just from numpy is great to do by yourself. Try it if you haven't ! (it's good training for the exam)
- experiment with the regularization notebooks (from session 3)
- bonus: double descent?

## session 6

Lecture:
- PCA
- Kernels
- SVM


Tutorial:
- We did (6.2-SVM-showcase+exercises+corrections.ipynb), which has not a lot of hard coding to it, but allows to see SVMs and Kernels at work.

# informations:

- exam rules: consult 0-organization-rules.pdf and the annals from last years, esp. the 2021 and 2022 ones.

Also:
- for running codes on GPU: there are Nvidia GPUs in D104. You can try getting the proper (pytorch-able) env by doing:
cd /opt/anaconda3/bin
./python3

# Fundamental Principles of Machine Learning

Gitlab for the course Fundamental Principles of Machine Learning (FPML or TC0) in the CS Masters (M1 year), in the track *Artificial Intelligence* of the Paris Saclay University

The e-campus address is (for the quizz):

https://ecampus.paris-saclay.fr/course/view.php?id=115777#section-7


Uncomfortable with numpy ? Try these exercises:
https://www.machinelearningplus.com/python/101-numpy-exercises-python/


# Hint from a student from previous year:
"This class is one of the basics (with Applied Stats for instance) that really teach you what you will need later." So, spending time studying this class is a good investment for later: either you study now and do good at the exam, or you'll have to study the same stuff later in the year for the following classes.

"study regularly" -> very good idea.


# IMPORTANT: PRE-REQUISITES !

**PRE1 and PRE2 as prerequisites, and PRE4 is strongly recommended**. Note that **PRE1 and PRE2 are mandatory, i.e. you must attend them to be allowed to follow TC0/FPML**, except if you can argue that you are already very fluent in statistics (PRE1) and linear algebra (PRE2) (in that case, e-mail me).
**This class** (or an equivalent) **is a prerequisite for almost all other [AI] classes**.

# Dec 7th class (catch up to Nov 11th)

Catch up class: there will be None, because we could not find a single date that suits everyone.
But we will meet, for those who want, on Dec 7th at 10am in PUIO (I'll book a room) for Q&A session, doing exercises, etc (stuff not mandatory for the exam, but which may help those who need).
I made a poll to know how many want to attend this (if 0, I won't have to come just for this..): it's called "Attendance for Dec 7th" (on ecampus) https://ecampus.paris-saclay.fr/mod/choice/view.php?id=1051905


# What we did in class

## session 1 - GD+Linear Regression (+organizational stuff)

During the first session, we did (i give the paths to files from the gitlab):

- read together "the rules": 0-organization-rules-intro/0-organization-rules.pdf
- The main Lecture material was: 1-Regressions: lecture1-ML-vocab+LinReg.pdf (we reached page 10, pages 11 and 12 are addressed in the tutorial, so it's ok, the rest will be seen later)
- Still lecture material: 1-GradientDescent/Gradient Descent-demo-compute2gradients.ipynb  : I explained in detail GD and its pitfalls, in particular in 1D. We did not compute the 2D case but ou can do it at home.

In tutorial, we did (may depend slightly on the group you are in):

- 1-Regressions: TD-Regressions.pdf -> we did the 1.1.1, 1.1.2, maybe the 1.1.3 (it's not very different from those before if you understand how to vectorize everything),
- in terms of notebooks, you filled the TP1.1-LinearRegression-GradientDescent.ipynb (either skipping the naive version and going directly for trick of the ones, or not), some people did also the TP1.2-LinReg-d-dimensional.ipynb (which is very similar to TP1.1)

A few students did also attack the TP1.3-LinReg-3rd-order-Polynomial.ipynb

## session 2 - Perceptron

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




## session 5 - Maximum A Posteriori (MAP), a Multi-Class framework (OVR), Feature Maps (quickly)


Lecture:
- MAP (Maximum A Posteriori), in general (for any statistical inference)
- Ridge Regression interpreted as a prior on weights (MAP !)
- Elastic Net, Graphical Models : 2 words
And, taking from the folder "optional material from previous or missed sessions":
- multi-class classification: complete the last bits of Lecture1/2, that we forgot to cover ! (`2-Multi-class-classification-end.pdf`)
- feature maps, if time allows (`3-2FeatureMaps.pdf`)

Tutorial:
- from TD-regularizations.pdf, 3.4.a, 3.4.b Maximum A Posteriori (in general) and 3.5.b Maximum A Posteriori (for regularization) as well (the (3.5.a) was covered during the Lecture)
- (we did not have the tie for this) TP5.1-coding your own Lasso-subject.ipynb -> code it ! Here we use Objected Oriented Programming, i.e. nice lcasses in numpy, sklearn-style

## session 6

Lecture:
- PCA
- Kernels
- SVM


Tutorial:
- some attacked the PCA (see 6.3-PCA-from-scratch+overfitting-correction.ipynb) first. Especially the part where you re-code PCA just from numpy is great to do by yourself. Try it if you haven't ! (it's good training for the exam)
- some started with the SVM part (6.2-SVM-showcase+exercises+corrections.ipynb), which has not a lot of hard coding to it, but allows to see SVMs and Kernels at work.

### Solutions to exercices of session 6 (and all of them) are online !!

I did improve the solution to 3.4.b.

Note: I will improve the solution to the 3.5.b, which currently is not that good/clear.


# informations:

Several informations:
- corrections to TP6 are online
- improved corrections to TD5 are online too (exercise 3.4.b and 3.5.b, i.e the ones related to Laplace priors)

Also:
- quiz 5 is online, you'll be able to take it on Wednesday, from noon to 15h30pm (25 min quiz, 16 questions). It does count in the grade. Then you'll be able to practice more with it as you wish (after 16h30)
- Homework: (see previous messages) the knowledgeable platform will be available tonight ! Link is: https://nowledgeable.com/invitation/student/ada30c2cb5bf4e179791019ac4fb23b8 (you will need to create an account, it takes 2 minutes. Please try to use your @universite-paris-saclay.fr email)  The link works now, but some bugs may be corrected today. If you have bugs after this evening, you can report them to us, and especially to Laurent Cetinsoy:  https://discord.gg/cmUxK8Nw (discord preferred, otherwise, email to laurent.cetinsoy@nowledgeable.com )
- exam rules: consult 0-organization-rules.pdf and the annals from last years, esp. the 2021 one. The exam will be in B108, 13h30->16h30 (3h).

Also:
- for running codes on GPU: there are Nvidia GPUs in D104. You can try getting the proper (pytorch-able) env by doing:
cd /opt/anaconda3/bin
./python3
- TER: On Tuesday morning (10h30) I'll welcome the students who don't yet have an individual TER and are interested to shift from the collective one to an individual one. See my webpage: http://lptms.u-psud.fr/francois-landes/internships-phd/

# Assignment 1 Report

*Delete this italic guidance as you fill in each section. You'll be asked to
defend any of this without your code in front of you — write only what you
can actually explain.*

- **Name**: Shamil Mukhamedov
- **Student ID**: 20352
- **Email**: smukhkamedov.ieu2022@student.ie.edu
- **Group**: BBADBA 5B

## Dataset

*What is it, where did you get it, what does one row represent, how many
rows/columns, and why did you pick it.*

I chose a dataset that shows whether or not a person defaulted on their loans given variables such as age, whether or not they employed, amount for loan, interest on loan, the term (in months) during which the loan was supposed to be paid back.

I got this dataset from Kaggle, I downloaded the zip file and ran it locally from my laptop using VS-code. 

I picked it because it was a dataset that allowed for binary classification, and because we worked with datasets like these (not this exact dataset, as we never used Kaggle for loan datasets) in our previous classes; therefore, using a loan-default-related dataset would allow me to better understand the business implications so I am able to explain them in the report. 

The dataset has 255347 rows and 18. One of them is the target variable, the other is the loanID, so there are 16 variables that affect whether or not a customer may default on a loan. 

## Business / real-life framing

*The hypothetical scenario this model serves, and what that scenario implies
for how you built the pipeline — target definition, whether a time-based
split was necessary and why (or why not), which metric should drive the
decision threshold and why.*

The hypothetical scenario that my model serves is the ability to disapprove or approve loan requests given the probability that a customer will default on that loan given the 16 variables that they are required to disclose at the moment they are requesting the loan. 

When I asked you about the dataset, you asked me to clearly define what a default on a loan is for the context of my dataset: a 0 on the Default column signifies that the laon (specified in the LoanAmount column) was paid back in full + interest (specified in the InterestRate column) within the time frame stated in the LoanTerm column; per contra, a 1 in the Default column states that the loan was not paid back (including added interest) within the specified time frame (LoanTerm column). From my EDA, I saw that the usual loan time frames are between 2-5 years (24 and 60 months since the dataset measures LoanTerm in months). 

The target variable is the Default column, it is a binary column where a 0 means the loan was paid back, a 1 means the customer defaulted on their loan.



## Data preparation & feature engineering

*What you engineered and why, and any data-quality decisions you made along
the way — e.g. "segment X had defective data, so I excluded it and used a
population-average default for scope Y at inference time; the impact of
that choice is Z."*

## Modeling: three implementations, one model

*Which model (linear or logistic regression) and why. A results table
comparing scikit-learn, the manual PyTorch loop, and the standard
torch.nn.Module/torch.optim workflow, on the same test set, against the
naive baseline. Do the three agree? If not, why not?*

## Limitations & next steps

*Real limitations you found, and concretely how you'd address each one with
more time or data — not generic hedging.*

## Generative AI use disclosure

*Per the syllabus AI Policy: what you used and how, or "no AI content used."*

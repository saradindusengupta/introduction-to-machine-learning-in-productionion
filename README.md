# Introduction to machine learning in productionion

Course work for Coursera [MLOps specialization](https://www.coursera.org/learn/introduction-to-machine-learning-in-production)


# Notes

# Project Scoping

## Software Metrics

* Accuracy

- Latency (millisecond)

- Throughput (queries per second)

- Timeline

- Compute (GPU/CPU/ Memory)

- Budget

- Real-time or Batch

- Cloud or Edge

- Logging

- Security and Privacy

## Input Metrics

- Avg input length

- Avg input volume

- Number of missing values

- Avg image brightness

## Output Metrics

- Num of times returned Null

- Num of times user redoes search

- Num of times user switches to typing

- Click-through-rates(For web-search based models)

# Setting up a Baseline

- Human level performance

- Quick implementation

- Literature search for state-of-the-art

- Performance of older system

# Metrics for Error Analysis for each tag

- What fraction of error has that tag ?

- Of all that data with that tag, what percentage is misclassified ?

- What fraction of all the data has that tag ?

- Room for improvement with data with tag tag ?

- Human level performance with that tag.

# Prioritizing on what to work on from error analysis

- How much room for improvement there is ?

- How frequently that category appears ?

- How easy is it to improve accuracy in that category ?

- How important it is to improve that category ?

# Data Augmentation

## Goal

Create realistic samples that

- the algorithm does poorly on

- humans performs fairly well

## Checklist

- Does it sound realistic ?

- is the X to Y mapping clear, i.e., is human still able to recognise  it ?

- is the algorithm currently doing poorly on ?

## Can it hurt model performance

In the following situations, adding more data will not hurt the model performance

- If the model is large enough

- If there are very few ambiguity between x→ Y mapping

# Experiment Tracking

What to track during and after development

- Algorithm

- Datasets

- Hyper-parameters

- Evaluation Metric

# Definition of a Good data-set

- Covers important cases

- is defined consistently (mapping between x→y is unambigous)

- Has timely feedback from production data (distribution covers data drift and concept drift)

- is sized properly

# Definition of large/small data

- Small data (unstructured/structured) - < 10k

- Big data (unstructured/structured) - > 10k

# Measure Human-level-performance

- Estimate Bayes error/ irreducible error

# Balanced train/dev/test data-set

- For small data-sets, a balanced split between train, dev and test (as 30% each) would give better representation of their original distribution than a random split

- The same is not needed, when the data-set is large as simple random split would work fine in that scenario

# Single Machine Scheduling: Comparison of MILP Formulations

## Project Overview

This project investigates different Mixed Integer Linear Programming (MILP) formulations for the Single Machine Scheduling Problem with Weighted Tardiness Minimization.

The objective is to determine an optimal sequence of jobs on a single machine while minimizing the total weighted tardiness of all jobs.

The optimization models were implemented in Python using Gurobi.

## Formulations Implemented

1. APDV (Assignment Position Decision Variables)
2. LOV (Linear Ordering Variables)
3. CTV (Completion Time Variables)
4. TIV (Time Indexed Variables)

## Features

* Exact optimization using Gurobi
* Runtime comparison between formulations
* Schedule generation
* Gantt chart visualization
* Results exported to CSV files
* Performance evaluation of alternative MILP formulations

## Tools and Technologies

* Python
* Gurobi Optimizer
* Pandas
* Matplotlib

## Problem Description

Given a set of jobs with:

* Processing times
* Due dates
* Weights

the objective is to find the job sequence that minimizes total weighted tardiness:

Minimize:

Σ wj × Tj

where:

Tj = max(0, Cj − dj)

Cj = completion time of job j

dj = due date of job j

wj = priority weight of job j

## Output

The project generates:

* Optimal job schedules
* Total weighted tardiness
* Solver runtime statistics
* Comparative analysis of four MILP formulations
* Gantt chart visualizations

## Learning Outcomes

This project demonstrates:

* Mathematical Optimization
* Operations Research
* Scheduling Theory
* MILP Modeling
* Computational Performance Analysis
* Optimization using Gurobi

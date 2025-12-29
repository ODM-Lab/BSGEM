# An Exact Optimization Approach for Single-Machine Scheduling under Periodic Unavailability: A Binary Search-Guided Framework

## 📂 Input Data for Reproducibility

This repository provides the benchmark instances used in our computational experiments.

The instances are based on the LOW and MOD benchmark sets from \citet{perez2018single} and are shared to ensure full reproducibility of our results.

---

## 🔍 Dataset Description

We use two sets of benchmark instances—referred to as the **LOW** set and **MOD** set—from \citet{perez2018single}. They consider fourteen different job sizes,

$$
n \in \{10, 20, 30, 40, 50, 60, 70, 80, 90, 100, 150, 200, 250, 300\},
$$

and assume that each job processing time follows a uniform distribution,

$$
p_j \sim U[1, 50].
$$

For each job size, **50 instances** are generated. For each instance, the periodic availability parameter $T$ is sampled from:

- **LOW set**: $$T \sim U[150, 200]$$  
- **MOD set**: $$T \sim U[50, 100]$$

This yields **700 instances per dataset**, and **1,400 instances in total**.

For reproducibility, we provide the benchmark instances used in our experiments (LOW and MOD) in this repository.

---

## 🧱 Data Structure

The dataset is organized by difficulty level (LOW / MOD) and job size $n$. Each folder contains 50 instances for the corresponding job size.

```text
.
├── LOW/
│   ├── n10/
│   │   ├── inst_001.txt
│   │   ├── inst_002.txt
│   │   └── ...
│   ├── n20/
│   │   ├── inst_001.txt
│   │   └── ...
│   └── ...
├── MOD/
│   ├── n10/
│   │   ├── inst_001.txt
│   │   └── ...
│   ├── n20/
│   │   ├── inst_001.txt
│   │   └── ...
│   └── ...
└── README.md

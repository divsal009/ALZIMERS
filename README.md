# Comparator-Aware 3D Deep Learning Framework for Structural MRI Classification Across Alzheimer’s Disease, Healthy Control, and Bipolar Disorder Cohorts

This repository provides the implementation of a comparator-aware 3D deep learning framework for structural MRI classification across Alzheimer’s Disease (AD), Healthy Control (HC), and Bipolar Disorder (BD) cohorts.

The framework is designed for multiclass classification using preprocessed T1-weighted structural MRI volumes, with an additional derived AD-versus-HC binary evaluation. The implementation follows a strict subject-wise evaluation strategy to reduce data leakage and support more reliable neuroimaging model assessment.

## Paper Title

**A Comparator-Aware 3D Deep Learning Framework for Structural MRI Classification Across Alzheimer’s Disease, Healthy Control, and Bipolar Disorder Cohorts**

## Overview

MRI-based Alzheimer’s disease classification is commonly evaluated as a binary AD-versus-HC problem. However, such a setting may oversimplify the clinical problem because non-AD conditions can introduce structural brain variation that complicates discrimination.

This project extends the evaluation setting by including Bipolar Disorder as a non-AD comparator cohort. The aim is to assess whether a 3D deep learning model can distinguish Alzheimer’s disease not only from healthy control anatomy, but also from structurally variable non-AD cases.

The framework includes:

- Subject-wise data partitioning
- Robust intensity normalisation
- Volumetric resizing to a common 3D input size
- Conservative training-time augmentation
- Dual-path 3D convolutional architecture
- Squeeze-and-excitation channel recalibration
- Gated feature fusion
- Multi-seed ensemble learning
- Test-time augmentation
- Scan-level and subject-level evaluation
- Multiclass and AD-versus-HC binary metrics

## Dataset

The experiments use the public Zenodo dataset:

**Alzheimer’s Disease versus Bipolar Disorder versus Health Control MRI data and processed results**

Zenodo record:

```text
https://zenodo.org/records/3935636

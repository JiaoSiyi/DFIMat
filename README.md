# DFIMat: Decoupled Flexible Interactive Matting in Multi-Person Scenarios

[Siyi Jiao]<sup>1\*</sup>, [Wenzheng Zeng](https://scholar.google.com.sg/citations?hl=en&user=RDTJO-4AAAAJ)<sup>1*</sup>, [Changxin Gao](https://scholar.google.com/citations?user=4tku-lwAAAAJ&hl=zh-CN&oi=ao)<sup>2</sup>, [Nong Sang](https://scholar.google.com/citations?user=ky_ZowEAAAAJ&hl=zh-CN&oi=ao)<sup>2†</sup>.

School of AIA, Huazhong University of Science and Technology

This repository contains the official implementation of the ACCV 2024 paper "DFIMat: Decoupled Flexible Interactive Matting in Multi-Person Scenarios".

## Overview
Interactive portrait matting refers to extracting the soft portrait from a given image that best meets the user's intent through their inputs.
Existing methods often underperform in complex scenarios, mainly due to three factors. (1) Most works apply a tightly coupled network that directly predicts matting results, lacking interpretability and resulting in inadequate modeling. (2) Existing works are limited to a single type of user input, which is ineffective for intention understanding and also inefficient for user operation. (3) The multi-round characteristics have been under-explored, which is crucial for user interaction. To alleviate these limitations, we propose DFIMat, a decoupled framework that enables flexible interactive matting. Specifically, we first decouple the task into 2 sub-ones: localizing target instances by understanding scene semantics and the flexible user inputs, and conducting refinement for instance-level matting. We observe a clear performance gain from decoupling, as it makes sub-tasks easier to learn, and the flexible multi-type input further enhances both effectiveness and efficiency. DFIMat also considers the multi-round interaction property, where a contrastive reasoning module is designed to enhance cross-round refinement.
Another limitation for multi-person matting task is the lack of training data. We address this by introducing a new synthetic data generation pipeline that can generate much more realistic samples than previous arts. A new large-scale dataset SMPMat is subsequently established. Experiments verify the significant superiority of DFIMat. With it, we also investigate the roles of different input types, providing valuable principles for users. Our code and dataset will be public.

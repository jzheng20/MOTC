## Handling The Non-Smooth  Challenge  in Tensor SVD: A Multi-Objective Tensor Recovery Framework


This repository contains the official codes for "Handling The Non-Smooth Challenge in Tensor SVD: A Multi-Objective Tensor Recovery Framework".


In this work, we introduce a new  tensor recovery model  with a  learnable   tensor nuclear norm to address such challenge. 
We develop a new optimization algorithm named Alternating Proximal Multiplier Method (APMM)  to solve the proposed tensor completion model  iteratively. Theoretical analysis  demonstrates  the convergence of the proposed APMM to the Karush–Kuhn–Tucker (KKT)  point of the  optimization problem.  In addition,  we propose a  multi-objective tensor recovery framework  based on  APMM to efficiently  explore the correlations of tensor data across its various dimensions, providing a new perspective on extending the t-SVD-based method to higher-order tensor cases. Numerical experiments demonstrated the effectiveness of the proposed method in   tensor completion.


#### Requirements
MATLAB 2022b: Ensure MATLAB is installed on your system. This codebase is compatible with MATLAB 2022b version. 


#### Provided datasets
We include CIFAR10 and CIFAR100 datasets for experimental reproduction. These datasets are located under the ./Data/ directory. Due to capacity constraints, only a subset of these datasets is provided. 

- CIFAR10
  
  ./Data/CIFAR10_test_img_500_.mat
  
- CIFAR100

  ./Data/CIFAR100_test_500_.mat

#### Codes for this paper (MOTC)
Here we provide the commands for running on the terminal. Make sure that you are located under ./MOTC_codes/ directory (Windows or Ubuntu).



  
- MOTC
  
  ./MOTC/fun_DemoBSD_TC_SL_NSGAii.m
  
  **How to run on CIFAR10 dataset**:
  ```
  cd MOTC
  matlab -nodisplay -nosplash -nodesktop -r "fun_DemoBSD_TC_SL_NSGAii('./','./Data',{'/CIFAR10_test_img_500_.mat'},true,0.3,10,50); exit;"
  ```
  **How to run on CIFAR100 dataset**:
  ```
  cd MOTC
  matlab -nodisplay -nosplash -nodesktop -r "fun_DemoBSD_TC_SL_NSGAii('./','./Data',{'/CIFAR100_test_500_.mat'},true,0.3,10,50); exit;"
  ```



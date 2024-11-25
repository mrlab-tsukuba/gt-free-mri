# Ground-truth-free deep learning approach for accelerated quantitative parameter mapping with Memory Efficient Learning

## Repository Description

This repository contains a portion of the data used in the study **"Ground-truth-free deep learning approach for accelerated quantitative parameter mapping with Memory Efficient Learning,"** to ensure reproducibility.

## Experiments

- **Experiment 1**: Multi Spin Echo (MSE)  
- **Experiment 2**: Variable Flip Angle (VFA)  
- **Experiment 3**: Quantitative Double Echo Steady State (qDESS)  

## File Structure

### 1. `(sequence name).csv`
These files provide evaluations of the reconstructed images based on three metrics:
- **PSNR**
- **SSIM**
- **MSE**

Contrast numbers are labeled in the format `#1`, `#2`, ..., etc.

### 2. `(sequence name)-map.csv`
These files contain evaluation results of quantitative maps using **NRMSE**.  
- **Experiment 1 & 2**:  
  - Evaluations are performed on the all region as well as specifically on **Gray Matter** and **White Matter**.  
- **Experiment 3**:  
  - Evaluations include results for six types of masks provided in the **SKM-TEA dataset**, as well as results for the all masked region.

**Note**: If a region is not present within a slice, the corresponding data is left blank.

The corresponding masks are as follows:

**#0**: All Region  
**#1**: Patellar Cartilage  
**#2**: Femoral Cartilage  
**#3**: Tibial Cartilage - Medial  
**#4**: Tibial Cartilage - Lateral  
**#5**: Meniscus - Medial  
**#6**: Meniscus - Lateral  
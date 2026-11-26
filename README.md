# FPP Hackathon Repository

## Introduction
This repository documents the results of a hackathon conducted as part of the "Fundamentals of Parallel Programming" (FPP) course. The primary goal of this hackathon was to achieve portability and performance improvements for a sequential codebase through parallelization techniques, utilizing tools like CUDA, OpenMP, and other parallel computing frameworks.

## Tools Used
- **CUDA**: the sequential 2D Laplacian filter was parallelized for one GPU.
- **CUDA with NCCL**: a second version splits the work across two GPUs.

The team chose CUDA over the other options in the course because it was the easiest to use and gave the largest speedup.

## Result
On a 46340 × 46340 input, the single-GPU CUDA version ran in 1.49 s against 29.32 s for the sequential code, a 19.68× speedup. The notebook also has timings and speedups for inputs from 1024 × 1024 upwards.

## Notebooks
The primary notebook containing all the codes, experiments, and analyses is [Laplacian_Filter_Problem_Hackathon_PT.ipynb](Laplacian_Filter_Problem_Hackathon_PT.ipynb).

## Contributors
The team at the HPC hackathon of Senai Cimatec, second semester of 2023:
- Antônio Horácio Magalhães
- Leonardo Rodrigues
- Orlando Mota Pires

## License
This project is licensed under the [MIT License](LICENSE).

# SomeUsefulTips
Some useful tips 

### pytorch-geometric
1. g++ version should larger than 4.9 or torch-scatter cannot work well even if it had been installed successfully.
2. if CUDA < 10.0 --> runnning any code on gpu will report an error: "sum_cuda" not implemented for 'Bool'. Just add .int() before any .sum(). Everything will run correctly.
e.g.: mask.sum() --> mask.int().sum()

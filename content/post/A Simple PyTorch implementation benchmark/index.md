---
title: A Simple PyTorch Implementation Benchmark
authors:
- admin
tags: ['deep learning', 'Web3']
categories: ['deep learning', 'Web3']
projects: ['Deep Learning']
date: 2023-04-10
math: true
diagram: true
highlight: true
image:
  placement: 3
  caption: 'Author By Z. Cao'
---

## Introduction
Welcome to my latest blog post, where I will be introducing a basic benchmark for PyTorch, the popular deep learning library. As a machine learning enthusiast, I understand the importance of measuring the performance of different hardware setups for deep learning tasks. By comparing the capabilities of various CPUs and GPUs, we can better understand the trade-offs and make more informed decisions when building our machine learning infrastructure.

In this post, I will present the results of a basic PyTorch benchmark that I ran on various CPUs and GPUs. I will discuss the performance of these hardware components in terms of iterations per second (it/s), and provide some insights into the differences observed.


## Code
```python
from tqdm import tqdm
import torch
import os,sys

# os.environ['CUDA_VISIBLE_DEVICES']='4'

# device=torch.device("cuda:4" if torch.cuda.is_available() else "cpu")
# print(device)

@torch.jit.script
def foo():
    x = torch.ones((1024 * 12, 1024 * 12), dtype=torch.float32)
    y = torch.ones((1024 * 12, 1024 * 12), dtype=torch.float32)
    x = x.cuda()
    y = y.cuda()
    z = x + y
    return z


if __name__ == '__main__':
    z0 = None
    for _ in tqdm(range(10000000000)):
        zz = foo()
        if z0 is None:
            z0 = zz
        else:
            z0 += zz
```


## Results

The following are the results obtained from the benchmarking experiment: 

(Updated 20/Apr)

| Hardware Component    | Performance (it/s) |
|-----------------------|--------------------|
| Nvidia 3090 GPU       | 670                |
| AMD Ryzen 9 3900X CPU | 21                 |
| Apple M1 CPU          | 48                 |
| Server CPU            | 74                 |
| Server GPU GTX1080Ti  | 300                |
| Server GPU (Overheat) | 55                 |
| Tencent Cloud         | 75                 |
| IIAIM Node GPU01 RTX3080 | 402            |
| Tencent VENUS V100 GPU | 677               |
| AMD Ryzen 5 5600G CPU | 25                 |
| Nvidia RTX3060 GPU    | 320                |

## Analysis

From the results, we can observe that GPUs generally outperform CPUs in terms of performance when running PyTorch tasks. For instance, the Nvidia 3090 GPU achieved 670 it/s, which is 6.8% of its performance when running on a CPU. This is a remarkable improvement, and demonstrates the power of GPUs for deep learning tasks.

When comparing different CPUs, we can see that the Apple M1 and Server CPU show better performance than the AMD Ryzen 9 3900X and Ryzen 5 5600G. However, the difference in performance between these CPUs is not as significant as the difference between GPUs.

On the GPU side, the Nvidia RTX3090 and Tencent VENUS V100 show the highest performance, followed by the IIAIM Node GPU01 RTX3080 and Nvidia RTX3060. Interestingly, the Server GPU GTX1080Ti and the overheat variant show comparatively lower performance, suggesting that thermal management plays a crucial role in GPU performance.

## Conclusion

In conclusion, this basic PyTorch benchmark highlights the advantages of using GPUs for deep learning tasks over CPUs. The performance gap between GPUs and CPUs is significant, and it is essential to choose the right hardware for your specific machine learning projects. It is also important to consider factors such as thermal management when selecting a GPU to ensure optimal performance.

As a final note, we hope to see further support for GPUs and neural engines in the near future, which could potentially unlock even greater performance gains for deep learning tasks.









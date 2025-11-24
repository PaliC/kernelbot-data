---
configs:
- config_name: submissions
  data_files: "submissions.parquet"
- config_name: successful_submissions
  data_files: "successful_submissions.parquet"
- config_name: leaderboards
  data_files: "leaderboards.parquet"
tags:
- code
license: mit
---

This is the dataset that was created from the first and second AMD $100K kernel competitions, containing roughly 110K kernels for fp8-gemm, moe, mla, all2all, gemm+reducescatter, and allgather+gemm optimized to run on MI300. Learn more at gpumode.com/v2/news

To see the full list of kernel competitions we've ran and are running you can checkout https://github.com/gpu-mode/reference-kernels which also contains details on reference kernels and their input shapes and distributions

We are planning on adding kernels optimized for NVFP4 on Blackwell next

If you use this dataset in your work, please cite:

```bibtex
@inproceedings{
  zhang2025kernelbot,
  title={KernelBot: A Competition Platform for Writing Heterogeneous {GPU} Code},
  author={Alex L Zhang and Matej Sirovatka and Erik Schultheis and Benjamin Horowitz and Mark Saroufim},
  booktitle={Championing Open-source DEvelopment in ML Workshop @ ICML25},
  year={2025},
  url={https://openreview.net/forum?id=bq9U4dmuyJ}
}
```

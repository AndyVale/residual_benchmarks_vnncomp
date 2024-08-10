# <a href="https://github.com/shizhouxing/ViT_vnncomp2023">A ViT benchmark for VNNCOMP2023</a>

We propose a benchmark on verifying Vision Transformers (ViTs).
The aim of this benchmark is to encourge the development of
verification techniques for Transformer based models, with
its iconic self-attention structure.

We trained relatively small ViTs either by pure PGD training
or PGD training combined with a small proportion of IBP loss.
The layer normalization in the ViTs has been replaced by batch normalization,
due to the difficulty of verifying layer noramlization identified by prior works.

We consider robustness verification with a Linf perturbation on 
CIFAR-10 with eps=1/255 at test time.
We have filtered the CIFAR-10 test set to exclude instances where
either adversarial examples can be found or vanilla CROWN can already easily verify.
We included normalized input examples in this repo to avoid normalization differences
in proprocessing.

## Model structure and information

| Model | `PGD_2_3_16` | `IBP_3_3_8` |
| ----- | ------------ | ----------- |
| Layers | 2 | 3 |
| Attention heads | 3 | 3 |
| Patch size | 16 | 8 |
| Training method | Pure PGD training | PGD training with (0.01 * IBP loss) |
| Training epsilon | 2/255 | 1/255 |
| Clean accuracy | 59.78% | 62.21%|

## Reference

If you use this benchmark, please kindly cite our following paper:
```
@article{shi2023generalnonlinear,
  title={Formal Verification for Neural Networks with General Nonlinearities via Branch-and-Bound},
  author={Shi, Zhouxing and Jin, Qirui and Kolter, J Zico and Jana, Suman and Hsieh, Cho-Jui and Zhang, Huan},
  journal={2nd Workshop on Formal Verification of Machine Learning (WFVML 2023)},
  year={2023}
}
```

### --- List of all vit_2023 [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### ibp_3_3_8.onnx 
	Number of parameters: 68266 
	Node types: ['ConstantOfShape' 'Gemm' 'Concat' 'Conv' 'BatchNormalization' 'Gather' 'Shape' 'Unsqueeze' 'ReduceMean' 'Softmax' 'Slice' 'Mul' 'Transpose' 'Relu' 'Add' 'Constant' 'Reshape' 'MatMul']

#### pgd_2_3_16.onnx 
	Number of parameters: 76186 
	Node types: ['ConstantOfShape' 'Gemm' 'Concat' 'Conv' 'BatchNormalization' 'Gather' 'Shape' 'Unsqueeze' 'ReduceMean' 'Softmax' 'Slice' 'Mul' 'Transpose' 'Relu' 'Add' 'Constant' 'Reshape' 'MatMul']


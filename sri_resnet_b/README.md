# <a href = "https://github.com/mnmueller/vnn_comp_22_bench_sri"> sri_resnet_b </a>

**Proposed by:** The MN-BaB team

**Motivation:** While in previous instantiations of the VNN-COMP, many benchmarks considered different architectures, thus allowing judgment of the effect of architecture changes on the (relative) performance of different verifiers, none allowed for a direct comparison of the effect of different training methods. To enable such a comparison, we propose two benchmarks considering the same network architecture, trained using adversarial training of different strengths.

**Networks:** We consider two residual ReLU networks with three ResBlocks, preceded by one convolutional layer and followed by two fully connected layers, yielding a total of eight ReLU layers. Both networks were trained using adversarial training, with the "A" version of the benchmark using a weaker attack compared to the "B" version.

### --- List of all sri_resnet_b [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2022_benchmarks'> vnncomp2022_benchmarks </a>)---

#### resnet_3b2_bn_mixup_ssadv_4.0_bs128_lr-1_v2.onnx 
	Number of parameters: 354488 
	Node types: ['Gemm' 'Conv' 'Relu' 'Add' 'Reshape']


# <a href ="https://github.com/ChristopherBrix/vnncomp2024_tinyimagenet_benchmark">TinyImageNet Neural Network Verification Benchmark for VNN-COMP 2024</a>

This is the re-proposed TinyImageNet benchmark for VNN-COMP 2024. The original benchmark [cifar100_tinyimagenet](https://github.com/Lucas110550/CIFAR100_TinyImageNet_ResNet) was from VNN-COMP 2022.

To reduce complexity to improve its accessibility to new tools and new VNN-COMP participants,
this TinyImageNet model is separated as a different benchmark, since not all tools can handle large model/data like this.
The model contain FC, conv, and ReLU layers only.

For more information about the models, you can check out the original repo in 2022 (here, we only kept the `TinyImageNet_resnet_medium` model only; other models were removed to reduce complexity).


### --- List of all tinyimagenet [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### TinyImageNet_resnet_medium.onnx 
	Number of parameters: 3616144 
	Node types: ['Gemm' 'BatchNormalization' 'Conv' 'Flatten' 'Relu' 'Add']


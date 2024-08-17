# <a href = "https://github.com/ChristopherBrix/vnn-comp-2022-Carvana-unet"> carvana_unet_2022<a>

A set of simplified Unet Benchmarks on Carvana for Neural Network Verification

We propose a new set of benchmarks of simplified unet on Carvana for neural network verification in this repository.

Motivation

Currently, most networks evaluated in the literature are focusing on image classfication. However, in many practical scenarios, e.g. autonomous driving, people pay more attention to object detection or semantic segmentation. Considering the complexity of the object detection, we propose a new set of simplified Unet (model one: four Conv2d layers followed with BN and ReLu; model two: add one AveragePool layer and one TransposedConv Upsampleing layer on the model one ). We advocate that tools should handle more practical architectures, and the simplified Unet is the first step towards this goal.

More details in the original repo...

### --- List of all carvana_unet_2022 [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2022_benchmarks'> vnncomp2022_benchmarks </a>)---

#### unet_simp_small.onnx 
	Number of parameters: 149570 
	Node types: ['Cast' 'Conv' 'OneHot' 'Gather' 'Softmax' 'Equal' 'ReduceSum' 'Slice' 'Relu' 'Transpose' 'ArgMax' 'Constant']

#### unet_upsample_small.onnx 
	Number of parameters: 329987.0 
	Node types: ['Pad' 'ConvTranspose' 'Softmax' 'Slice' 'AveragePool' 'ArgMax' 'Reshape' 'Cast' 'ConstantOfShape' 'Gather' 'Shape' 'Equal' 'Constant' 'Concat' 'Conv' 'Div' 'OneHot' 'ReduceSum' 'Relu' 'Transpose' 'Sub' 'Unsqueeze']


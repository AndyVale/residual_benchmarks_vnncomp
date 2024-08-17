# <a href ="https://github.com/Khoury-srg/VNNComp23_NN4Sys"> Characterizing Neural Network Verification for Systems with NN4SysBench </a>

We propose a new set of benchmarks for neural network verification for systems (NN4Sys) in this repository. This suite includes verification benchmark for learned index, learned cardinality and learned video stream, which are three tasks that apply neural networks to solve traditional tasks for systems.

More details in the original repo...

### --- List of all nn4sys_2023 [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### mscn_128d.onnx 
	Number of parameters: 102529 
	Node types: ['Div' 'Gemm' 'Concat' 'Sigmoid' 'ReduceSum' 'Slice' 'Mul' 'Relu' 'Add' 'Constant' 'Split' 'MatMul']

#### mscn_128d_dual.onnx 
	Number of parameters: 154881 
	Node types: ['Div' 'Gemm' 'Concat' 'Sigmoid' 'ReduceSum' 'Slice' 'Mul' 'Relu' 'Add' 'Sub' 'Constant' 'Split' 'MatMul']

#### mscn_2048d.onnx 
	Number of parameters: 25233409 
	Node types: ['Div' 'Gemm' 'Concat' 'Sigmoid' 'ReduceSum' 'Slice' 'Mul' 'Relu' 'Add' 'Constant' 'Split' 'MatMul']

#### pensieve_big_parallel.onnx 
	Number of parameters: 527494 
	Node types: ['Div' 'Gemm' 'Concat' 'Conv' 'Gather' 'ReduceSum' 'Slice' 'Relu' 'Flatten' 'Sub' 'Constant' 'Reshape' 'Split' 'Pow' 'MatMul']

#### pensieve_big_simple.onnx 
	Number of parameters: 527494 
	Node types: ['Gemm' 'Concat' 'Conv' 'Gather' 'Slice' 'Relu' 'Constant' 'Reshape']

#### pensieve_mid_parallel.onnx 
	Number of parameters: 264454 
	Node types: ['Div' 'Gemm' 'Concat' 'Conv' 'Gather' 'ReduceSum' 'Slice' 'Mul' 'Relu' 'Flatten' 'Sub' 'Constant' 'Reshape' 'Split' 'MatMul']

#### pensieve_mid_simple.onnx 
	Number of parameters: 264454 
	Node types: ['Gemm' 'Concat' 'Conv' 'Gather' 'Slice' 'Relu' 'Constant' 'Reshape']

#### pensieve_small_parallel.onnx 
	Number of parameters: 103174 
	Node types: ['Div' 'Gemm' 'Concat' 'Gather' 'ReduceSum' 'Slice' 'Relu' 'Flatten' 'Sub' 'Constant' 'Reshape' 'Split' 'Pow' 'MatMul']

#### pensieve_small_simple.onnx 
	Number of parameters: 103174 
	Node types: ['Gemm' 'Concat' 'Gather' 'Slice' 'Relu' 'Add' 'Constant' 'Reshape' 'MatMul']


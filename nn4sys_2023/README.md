# <a href ="https://github.com/Khoury-srg/VNNComp23_NN4Sys"> Characterizing Neural Network Verification for Systems with NN4SysBench </a>

**Proposed by the α,β-CROWN team in collaboration with Cheng Tan and Haoyu He at Northeastern University.**

**Application:** The benchmark contains networks for database learned index and learned cardinality estimation, which map input from various dimensions to a single scalar output.

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

#### pensieve_mid_simple.onnx 
	Number of parameters: 264454 
	Node types: ['Gemm' 'Concat' 'Conv' 'Gather' 'Slice' 'Relu' 'Constant' 'Reshape']

#### pensieve_small_parallel.onnx 
	Number of parameters: 103174 
	Node types: ['Div' 'Gemm' 'Concat' 'Gather' 'ReduceSum' 'Slice' 'Relu' 'Flatten' 'Sub' 'Constant' 'Reshape' 'Split' 'Pow' 'MatMul']

#### pensieve_small_simple.onnx 
	Number of parameters: 103174 
	Node types: ['Gemm' 'Concat' 'Gather' 'Slice' 'Relu' 'Add' 'Constant' 'Reshape' 'MatMul']


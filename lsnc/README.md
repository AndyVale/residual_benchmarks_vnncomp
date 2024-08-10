# <a href ="https://github.com/shizhouxing/LSNC_VNNCOMP2024">VNN Benchmark: Lyapunov-Stable Neural Control</a>

This is a benchmark for [VNN-COMP 2024](https://sites.google.com/view/vnn2024).
The models come from the ICML 2024 paper on [Lyapunov-stable Neural Control for State and Output Feedback](https://arxiv.org/pdf/2404.07956).
The goal is to certify the Lyapunov stability of NN controllers in nonlinear dynamical systems within a region-of-intrest and a region-of-attraction.
Specifications for the benchmark are randomly generated and consist of random sub-regions within the original region-of-interest.
We adopt two models for the 2D quadrotor dynamical system with state feedback and output feedback, respectively.
Each model consists of a controller which is a shallow ReLU network, a Lyapunov function which is a quadratic function, and nonlinear operators modelling the dynamics of a 2D quadrotor. The model for output feedback further consists of a shallow LeakyReLU network as the observer.
The verification objective of the Lyapunov stability has been encoded in the ONNX graphs and VNNLIB specifications.

Details of the problem can be found in our paper, and please kindly cite the paper if you use this benchmark:

*Lujie Yang\*, Hongkai Dai\*, Zhouxing Shi, Cho-Jui Hsieh, Russ Tedrake, and Huan Zhang*
"[Lyapunov-stable Neural Control for State and Output Feedback: A Novel Formulation for Efficient Synthesis and Verification](https://arxiv.org/pdf/2404.07956.pdf)" (\*Equal contribution)

### --- List of all lsnc [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### quadrotor2d_output.onnx 
	Number of parameters: 406 
	Node types: ['ConstantOfShape' 'Div' 'Concat' 'Gemm' 'Shape' 'Gather' 'ReduceSum' 'Neg' 'LeakyRelu' 'Slice' 'Mul' 'Cos' 'Relu' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### quadrotor2d_state.onnx 
	Number of parameters: 210 
	Node types: ['Div' 'Gemm' 'Concat' 'ReduceSum' 'Neg' 'Slice' 'Sin' 'Mul' 'Cos' 'Relu' 'Add' 'Sub' 'Constant' 'MatMul']


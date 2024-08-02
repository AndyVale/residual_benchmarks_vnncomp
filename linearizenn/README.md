# LinearizeNN_benchmark2024

Run
----------------------

```bash
python3 generate_instances.py <seed>
```

Installation and requirement
----------------------

```bash
pip3 install -r requirements.txt
```


Description
----------------------
This is a benchmark of Linearize NN for VNNCOMP 2024.


Assuming having a neural network controller approximation with a piecewise linear model in the form of a set of linear models with added noise to account for local linearization error. The objective of this benchmark is to investigate the neural network output falls within the range we obtain from our linear model output plus some uncertainty. Given input $x \in X$ and output $Y = f_{NN}(x)$, the query is of the form: $A_{mat}\times X + b + U_{lb} \leq Y \leq A_{mat}\times X + b + U_{ub}$ for each linear model in its abstraction region.

The neural network controller we used in this benchmark is an image-based controller for an Autonomous Aircraft Taxiing System whose goal is to control an aircraft’s taxiing at a steady speed on a taxiway. This network was introduced  in the paper [Verification of Image-based Neural Network Controllers Using Generative Models](https://arxiv.org/abs/2105.07091). The neural network integrates a concatenation of the cGAN (conditional GAN) and controller, resulting in a unified neural network controller with low-dimensional state inputs. In this problem, the inputs to the neural network consist of two state variables and two latent variables. The aircraft’s state is determined by its crosstrack position (p) and heading angle error (θ) with respect to the taxiway center line. Two latent variables with a range of -0.8 to 0.8 are introduced to account for environmental changes.



### --- List of all linearizenn [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### AllInOne_10_10.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_120_120.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_120_30.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_120_50.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_30_30.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_30_80.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_50_120.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_50_50.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_80_30.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']

#### AllInOne_80_80.onnx 
	Number of parameters: 203002 
	Node types: ['Gemm' 'Concat' 'Slice' 'Relu' 'Constant' 'MatMul']


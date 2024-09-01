# <a href = "https://github.com/AI4OPT/ml4acopf_benchmark"> ml4acopf benchmark </a>

**Proposed by Haoruo Zhao, Michael Klaminkin, Mathieu Tanneau, Wenbo Chen, and Pascal Van Hentenryck (Georgia Institute of Technology), and Hassan Hijazi, Juston Moore, and Haydn Jones (Los Alamos National Laboratory).**

**Motivation:** Machine learning models are utilized to predict solutions for an optimization model known as AC Optimal Power Flow (ACOPF) in the power system. Since the solutions are continuous, a regression model is employed. The objective is to evaluate the quality of these machine learning model predictions, specifically by determining whether they satisfy the constraints of the optimization model. Given the challenges in meeting some constraints, the goal is to verify whether the worst-case violations of these constraints are within an acceptable tolerance level.

**Networks:** The neural network designed comprises two components. The first component predicts the solutions of the optimization model, while the second evaluates the violation of each constraint that needs checking. The first component consists solely of general matrix multiplication (GEMM) and rectified linear unit (ReLU) operators. However, the second component has a more complex structure, as it involves evaluating the violation of AC constraints using nonlinear functions, including sigmoid, quadratic, and trigonometric functions such as sine and cosine. This complex evaluation component is incorporated into the network due to a limitation of the VNNLIB format, which does not support trigonometric functions. Therefore, these constraints violation evaluation are included in the neural network.

More details in the orginal repo...

### --- List of all ml4acopf_2024 [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### 118_ieee_ml4acopf-linear-nonresidual.onnx 
	Number of parameters: 164199.0 
	Node types: ['Gemm' 'Concat' 'Gather' 'Slice' 'Mul' 'Relu' 'Transpose' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### 118_ieee_ml4acopf-linear-residual.onnx 
	Number of parameters: 164049.0 
	Node types: ['Div' 'Gemm' 'Concat' 'Gather' 'Slice' 'Floor' 'Mul' 'Relu' 'Transpose' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### 118_ieee_ml4acopf.onnx 
	Number of parameters: 163868 
	Node types: ['Slice' 'Sin' 'Cos' 'Where' 'ConstantOfShape' 'Gather' 'Sigmoid' 'Equal' 'Constant' 'Concat' 'Neg' 'Mul' 'Pow' 'Gemm' 'Relu' 'Transpose' 'Add' 'Sub' 'Expand' 'MatMul']

#### 14_ieee_ml4acopf-linear-nonresidual.onnx 
	Number of parameters: 4481.0 
	Node types: ['Gemm' 'Concat' 'Gather' 'Slice' 'Mul' 'Relu' 'Transpose' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### 14_ieee_ml4acopf-linear-residual.onnx 
	Number of parameters: 4331.0 
	Node types: ['Div' 'Gemm' 'Concat' 'Gather' 'Slice' 'Floor' 'Mul' 'Relu' 'Transpose' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### 14_ieee_ml4acopf.onnx 
	Number of parameters: 4150 
	Node types: ['Slice' 'Sin' 'Cos' 'Where' 'ConstantOfShape' 'Gather' 'Sigmoid' 'Equal' 'Constant' 'Concat' 'Neg' 'Mul' 'Pow' 'Gemm' 'Relu' 'Transpose' 'Add' 'Sub' 'Expand' 'MatMul']

#### 300_ieee_ml4acopf-linear-nonresidual.onnx 
	Number of parameters: 680345.0 
	Node types: ['Gemm' 'Concat' 'Gather' 'Slice' 'Mul' 'Relu' 'Transpose' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### 300_ieee_ml4acopf-linear-residual.onnx 
	Number of parameters: 680195.0 
	Node types: ['Div' 'Gemm' 'Concat' 'Gather' 'Slice' 'Floor' 'Mul' 'Relu' 'Transpose' 'Add' 'Sub' 'Constant' 'Unsqueeze' 'MatMul']

#### 300_ieee_ml4acopf.onnx 
	Number of parameters: 680014 
	Node types: ['Slice' 'Sin' 'Cos' 'Where' 'ConstantOfShape' 'Gather' 'Sigmoid' 'Equal' 'Constant' 'Concat' 'Neg' 'Mul' 'Pow' 'Gemm' 'Relu' 'Transpose' 'Add' 'Sub' 'Expand' 'MatMul']


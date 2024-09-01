# <a href ="https://github.com/loonwerks/vnncomp2023"> VNNComp2023 - Collins Aerospace benchmark problem </a>

## Content

[Collins Aerospace Applied Research & Technology](https://www.collinsaerospace.com/what-we-do/technology-and-innovation/applied-research-and-technology) provides a benchmark problem for the [2023 International Verifification of Neural Networks Competition (VNNComp)](https://sites.google.com/view/vnn2023). Proposed use case is an object detection system for unmanned aerial vehicles (UAVs) that perform maritime search and rescue missions. The benchmark is related to robustness against pixel modifications in the neighborhood of the objects to be detected by the system (e.g., persons, boats). The system contains a YOLOv5 nano neural network. Robustness properties are formulated on raw inputs and raw output tensors of YOLO, which are numerous, which makes the problem challenging.

For detailed documentation, refer to the "benchmark_description.pdf" available in the original repository.

### --- List of all collins_aerospace_benchmark [residual_net] networks (From :<a href = 'https://github.com/ChristopherBrix/vnncomp2024_benchmarks'> vnncomp2024_benchmarks </a>)---

#### yolov5nano_LRelu_640.onnx 
	Number of parameters: 1767283 
	Node types: ['Concat' 'Conv' 'Constant' 'Sigmoid' 'LeakyRelu' 'Mul' 'Resize' 'Transpose' 'Add' 'MaxPool' 'Reshape' 'Split' 'Pow']


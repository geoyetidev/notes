[Website](https://mlsysbook.ai/contents/benchmarking/benchmarking.html)

### Critical Objectives
* Performance assessment
* Resource evaluation (e.g. hardware)
* Validation and Verification
* Competitive analysis
* Credibility
* Regulation and Standardization 

Successful benchmarks have **community consensus**

Benchmarking can happen at different levels of granularity,  from individual activation function performance to end-to-end application performance and user experience. 
### Benchmark Types
+ System Benchmarks (e.g. hardware, training times, etc)
+ Model Benchmarks (e.g. "accuracy")
+ Data Benchmarks (e.g. quality, diversity)

### Benchmarking Components
+ Standardized Datasets
+ Pre-defined Tasks
+ Evaluation Metrics
+ Baselines and Baseline Models
+ Hardware and Software Specs
+ Environmental Conditions (e.g. power source, background processes
+ Reproducibility protocols (.e.g random seeds, hyper-parameters)
+ Result Interpretation (e.g. assessment of appropriateness of metric to various real-world use cases) 

## System Benchmarks: 
+ **Training Benchmarks** - System oriented. Usually care about optimizating for time or compute resources
+ **Inference Benchmarks**  - Model oriented. Cares about accuracy, precision, recall

### Training Benchmark Metrics
+ Training Time
+ Scalability
+ Resource Utilization
+ Memory Consumption
+ Energy Consumption
+ Throughput
+ Cost
+ Fault Tolerance/Robustness (of training process)
+ Reproducibility

#### Common Frameworks
+ [MLPerf Training Benchmark](https://github.com/mlcommons/training)
+ [AWNBench](https://dawn.cs.stanford.edu/benchmark/)
+ [Fathom](https://github.com/rdadolf/fathom)

### Inference Benchmarks
+ Accuracy
+ Latency
+ Throughput
+ Latency-Bounded Throughput (e..g how many video frames the system can process per second (throughput) while ensuring that the subtitles are displayed with no more than a 1-second delay (latency))
+ Energy Efficiency
+ Memory Usage

#### Common Frameworks
+ [MLPerf Inference Benchmark](https://github.com/mlcommons/inference)
+ [AI Benchmark](https://ai-benchmark.com/)
+ [OpenVINO toolkit](https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/overview.html):

## Model Benchmarks
### Historical Context
+ [MNIST dataset](https://www.tensorflow.org/datasets/catalog/mnist)
+ [ImageNet dataset](https://www.tensorflow.org/datasets/catalog/imagenet2012)
+ [Common Objects in Context (COCO) dataset](https://cocodataset.org/)
+ GPT-3 - Dataset not available

### Model Metrics
+ Accuracy (and associated problems)
+ Fairness (how does this model operate on different subgroups of the data - see why accuracy is not a good measure)
	+ [[AI Fairness 360]]
	+ [[Tensorflow - Fairness Indicators]]
+ Complexity (number of parameters, floating point operations per second)
+ Efficiency (e.g. system metrics)

## Data Benchmarks
"...the emphasis shifts to curating high-quality datasets that better reflect real-world complexity, developing more informative evaluation benchmarks, and carefully considering how data is sampled, preprocessed, and augmented. The goal is to optimize model behavior by improving the data rather than just optimizing metrics on flawed datasets."

Data-centric AI - improve data not code for better real-world performance
#### Data Issues
+ Labeling Errors
+ Noisy features
+ Representation imbalance (over representation of certain subsets)
+ Class imbalance (imbalanced class examples)
+ Biases

#### Emerging Frameworks
+ [[DataComp]]
+ [[DataPerf]] 


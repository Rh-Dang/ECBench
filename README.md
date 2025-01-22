# ECBench: A Holistic Embodied Cognition Benchmark
[[paper](https://arxiv.org/abs/2501.05031)]
[[dataset](data)]

## Abstract
The enhancement of generalization in robots by large vision-language models (LVLMs) is increasingly evident. Therefore, the embodied cognitive abilities of LVLMs based on egocentric videos are of great interest. However, current datasets for embodied video question answering lack comprehensive and systematic evaluation frameworks. Critical embodied cognitive issues, such as robotic self-cognition, dynamic scene perception, and hallucination, are rarely addressed. To tackle these challenges, we propose ECBench, a high-quality benchmark designed to systematically evaluate the embodied cognitive abilities of LVLMs. ECBench features a diverse range of scene video sources, open and varied question formats, and 30 dimensions of embodied cognition. To ensure quality, balance, and high visual dependence, ECBench uses class-independent meticulous human annotation and multi-round question screening strategies. Additionally, we introduce ECEval, a comprehensive evaluation system that ensures the fairness and rationality of the indicators. Utilizing ECBench, we conduct extensive evaluations of proprietary, open-source, and task-specific LVLMs. ECBench is pivotal in advancing the embodied cognitive capabilities of LVLMs, laying a solid foundation for developing reliable core models for embodied agents. 

## Dataset

The ECBench dataset consists of 4324 question answer pairs $(Q,A^*)$ and corresponding episode histories $H$.

The question-answer pairs are available in [data/ECBench_qa.json](data/ECBench_qa.json) and the episode histories can be downloaded by following the instructions [here](data).

## Baselines and Automatic Evaluation
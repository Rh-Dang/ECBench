# Benchmark Evaluation
This document provides instructions on how to conduct `ECBench evaluation` for your model. Follow the steps below to ensure that your model's outputs are correctly evaluated.

## Overview
To evaluate your model, you need to store the outputs in a specified format and then run a script that will handle the evaluation process. This requires setting specific environment variables before running the evaluation script.

## Steps for Evaluation
- Get Model Evaluation Results:

  - system prompt:
```
You are moving in an indoor environment. The image sequence is the scene you just saw. You are now staying at the last frame of the video. Please answer the question with one word or one sentence, as concise and accurate as possible.
```

- Format Model Outputs:

   - Ensure that the model outputs are saved in a JSON format where each result is stored under the key 'pred_answer'. Here is an example structure:

```
   [
       {
           "video_name": "dynamic_0000",
            "dimensions": "['Information_Change']",
            "video_source": "evs",
            "question_en_v2.2": "What contents on the whiteboard have changed during this period? The color of the word 'GOD', the color of the word 'SKY', the first line of the blue-font equation, the second line of the blue-font equation, the first line of the chemical reaction equation.?",
            "answer_en_v2.2": "The color of the word 'SKY' and the second line of the blue font equation.",
            "Partially correct answer": 0,
            "scene_type": [
                "meeting room"
            ],
            "source_dataset": "dynamic",
            "dataset_pth": "/mnt/group_data/zwq_data/embody_benchmark/dataset/dynamic/",
            "pred_answer": "The color of the word 'SKY'",
       }
       ...
   ]
```


## Setup Environment Variables:

Before running the evaluation script, you must set the following environment variables for GPT evaluation:
```
export GPT_ENDPOINT="your_endpoint_here"
export GPT_KEY="your_key_here"
```

## Run the Evaluation Script:

Execute the `eval.sh` script to start the evaluation process and specify the output file path in the `eval.sh`.

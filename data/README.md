# ECBench Dataset

The ECBench dataset includes questions, answers, and egocentric videos.

The question-answer pairs are in [ECBench_qa.json](ECBench_qa.json) and the instructions below describe how to download the episode histories.

## Download Episode Histories

Episode histories are sourced from [HM3D](https://aihabitat.org/datasets/hm3d), [ScanNet](http://www.scan-net.org), [MultiScan](https://3dlg-hcvc.github.io/multiscan/) and ECBench native videos.
Follow the instructions below to download the episode histories from the above sources.

### Hugging Face Download

The RGBD videos for ECBench are available in [hugging face](https://huggingface.co/datasets/RH-Dang/ECBench) . 

Your top-level directory structure should look like this:

```text
|- data
    |- rgb_video
        |- dynamic
            |- dynamic_0000.mp4
            |- dynamic_0001.mp4
            |- ...
        |- hallucination
            |- scene_0000_00.mp4
            |- ...
        |- hm3d
            |- hm3d_0000.mp4
            |- ...
        |- multiscan
            |- scene_00000_00.mp4
            |- ...
        |- scannet
            |- scene0000_00.mp4
            |- ...
    |- depth
        |- dynamic
            |- ...
        |- hallucination
        |- hm3d
        |- multiscan
        |- scannet

```

| Format | Size | 
| --- | --- | 
| RGB-only | 24.2 Gb |
| RGB-D | 16Gb Gb | 

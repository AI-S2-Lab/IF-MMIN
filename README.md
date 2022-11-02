# IF-MMIN

 
## Introduction
This is an implementation of the following paper.
> [Exploiting modality-invariant feature for robust multimodal emotion recognition with missing modalities.](https://arxiv.org/abs/2210.15359)
> Submitted to ICASSP'2023

Haolin Zuo, [Rui Liu *](https://ttslr.github.io/), [Jinming Zhao](https://scholar.google.com/citations?user=XskCnD8AAAAJ&hl=en), Guanglai Gao, [Haizhou Li](https://colips.org/~eleliha/).
 

[![arXiv](https://img.shields.io/badge/arXiv-Paper-<COLOR>.svg)](https://arxiv.org/abs/2210.15359)




# Environment

``` 
python 3.8.0
pytorch >= 1.0.0
```

# Usage

First you should change the data folder path in ```data/config``` and preprocess your data follwing the code in ```preprocess/```.

You can download the preprocessed feature to run the code.

+ For Training IF-MMIN on IEMOCAP:

    First training a model fusion model with all audio, visual and lexical modality as the pretrained encoder.

    ```bash
    bash scripts/CAP_utt_shared.sh AVL [num_of_expr] [GPU_index]
    ```

    Then

    ```bash
    bash scripts/CAP_IFMMIN.sh [num_of_expr] [GPU_index]
    ```


Note that you can run the code with default hyper-parameters defined in shell scripts, for changing these arguments, please refer to options/get_opt.py and the ```modify_commandline_options``` method of each model you choose.

# Download the features
Baidu Yun Link
IEMOCAP A V L modality Features
链接: https://pan.baidu.com/s/1WmuqNlvcs5XzLKfz5i4iqQ 提取码: gn6w 


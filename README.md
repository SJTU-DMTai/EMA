

# EMA

## Introduction
this is the official implementaion of EMA framework for the TKDE paper "A Framework for Elastic Adaptation of User Multiple Intents in Sequential Recommendation". The IMA version can be found in cloudcatcher/IMSR.


## Abstract
Recently, substantial research has been conducted on sequential recommendation, with the objective of forecasting the
subsequent item by leveraging a user’s historical sequence of interacted items. Prior studies employ both capsule networks and
self-attention techniques to effectively capture diverse underlying intents within a user’s interaction sequence, thereby achieving the
most advanced performance in sequential recommendation. However, users could potentially form novel intents from fresh interactions
as the lengths of user interaction sequences grow. Consequently, models need to be continually updated or even extended to adeptly
encompass these emerging user intents, referred as incremental multi-intent sequential recommendation. In this paper, we propose an
effective Incremental learning framework for user Multi-intent Adaptation in sequential recommendation called IMA, which augments
the traditional fine-tuning strategy with the existing-intents retainer, new-intents detector, and projection-based intents trimmer to
adaptively expand the model to accommodate user’s new intents and prevent it from forgetting user’s existing intents. Furthermore, we
upgrade the IMA into an Elastic Multi-intent Adaptation (EMA) framework which can elastically remove inactive intents and compress
user intent vectors under memory space limit. Extensive experiments on real-world datasets verify the effectiveness of the proposed
IMA and EMA on incremental multi-intent sequential recommendation, compared with various baselines.

## Requirement

```
pytorch == 1.14
python == 3.7
```

## Instruction
1, You can run the code by: 

```
python code/EMA.py
```

3, You can change customize the initial interest number K and \delta K in utils.Config.

# Result
In the following figure shows the result on Xlong.

![](/Xlong.png)

# Reference

Please cite our paper if you use this code.

```
@article{wang2024ema,
  title={A Framework for Elastic Adaptation of User Multiple Intents in Sequential Recommendation},
  author={Zhikai Wang and Yanyan Shen},
  journal={TKDE},
}
```

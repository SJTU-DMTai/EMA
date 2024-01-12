

# EMA

this is the official implementaion of EMA framework for the TKDE paper "A Framework for Elastic Adaptation of User Multiple Intents in Sequential Recommendation". The IMA version can be found in cloudcatcher/IMSR.
## Architecture

![](/arch.png)


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

4, result on Electronic:

![](/Electronic-NDCG.png)

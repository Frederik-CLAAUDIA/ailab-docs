On AI-LAB, we have a ready-to-use [PyTorch](https://pytorch.org/) container image. This means that you can quickly access PyTorch's functionality within the AI-LAB environment without needing to install or configure the software yourself.

First, copy the PyTorch container image from the container directory on AI-LAB to your own user directory:

```console
cp /ceph/container/pytorch_24.03-py3.sif .
```

<span style="font-weight: 600;">Note! </span>PyTorch might be newer version at this time. Check the latest available version in the container directory.

You can run PyTorch scripts using Singularity to execute within the container. Below is an example of running a PyTorch script with 1 GPU allocated:

```
srun --gres=gpu:1 singularity exec --nv pytorch_24.03-tf2-py3.sif python3 your_script.py
```
#### Checkpointing
Checkpointing is a technique used to ensure that your computational jobs can be resumed from a previously saved state in case of interruptions or failures. Checkpointing in PyTorch can be used to save the state of your model at various points, enabling you to resume training from a specific epoch in case of interruptions or to fine-tune models from previously saved states. [This guide](/additional-guides/checkpointing/#pytorch-model-checkpointing) demonstrates checkpoint implementation in PyTorch.
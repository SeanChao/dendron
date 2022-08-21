---
id: yd2w94lhzi0zhafo0yskzq3
title: Model_size
desc: ''
updated: 1651147800153
created: 1651147769383
---

Get the model size (the number of parameters) for pytorch and tensorflow:

```python
sum(p.numel() for p in model.parameters() if p.requires_grad) for pytorch and
np.sum([np.prod(v.shape) for v in tf.trainable_variables]) for tensorflow
```

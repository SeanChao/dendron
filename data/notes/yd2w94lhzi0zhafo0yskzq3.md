
Get the model size (the number of parameters) for pytorch and tensorflow:

```python
sum(p.numel() for p in model.parameters() if p.requires_grad) for pytorch and
np.sum([np.prod(v.shape) for v in tf.trainable_variables]) for tensorflow
```

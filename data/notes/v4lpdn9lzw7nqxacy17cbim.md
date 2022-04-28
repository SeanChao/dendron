
## Hex

### Bytes Array to Hex String

pad with `0` to length of `2` in hex

```python
''.join([f"{b:02x}" for b in bytes_array])
# [1, 255] -> '01ff'
```

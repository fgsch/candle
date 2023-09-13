# candle-t5

Generates embeddings using a T5 model. It doesn't support generation yet.

```bash
$ cargo run --example t5 -- --model-id t5-large --prompt 'how tall is obama' --n 1
Loaded and encoded 2.014244792s
[[[-0.3174, -0.1462,  0.0065, ..., -0.0579, -0.0581,  0.1387],
  [-0.2905, -0.1945, -0.0685, ..., -0.2457, -0.5137, -0.1760],
  [-0.0591, -0.0213, -0.0241, ..., -0.0210,  0.0491, -0.0300],
  ...
  [-0.4333,  0.0027, -0.0609, ...,  0.3069, -0.2252,  0.3306],
  [-0.1458,  0.1323, -0.0138, ...,  0.3000, -0.4550, -0.0384],
  [ 0.0397,  0.0485, -0.2373, ...,  0.2578, -0.2650, -0.4356]]]
Tensor[[1, 9, 1024], f32]
Took 2.1363425s
```
# mrstat-toolkit

## Structure

```
mrstat-toolkit/
├── python/
│   └── neuralbloch/        # Train and export the surrogate model (PyTorch)
├── julia/
│   └── NeuralBloch.jl/     # Run the exported model on NVIDIA GPUs (TensorRT)
├── external/
│   └── MRSTAT.jl/          # MR-STAT reconstruction (git submodule)
├── pyproject.toml          # uv workspace
└── Project.toml            # Julia workspace
```

Each package has its own README with the requirements and the usage:

- [`python/neuralbloch`](python/neuralbloch/README.md)
- [`julia/NeuralBloch.jl`](julia/NeuralBloch.jl/README.md)
- [`external/MRSTAT.jl`](external/MRSTAT.jl/README.md)

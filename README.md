# mrstat-toolkit

Tools for MR-STAT: the NeuralBloch surrogate model of Bloch simulations and the MR-STAT reconstruction.

[![lint](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/lint.yml)

[![python-ci](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/python-ci.yml/badge.svg?branch=main)](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/python-ci.yml)
[![python-docs](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/python-docs.yml/badge.svg?branch=main)](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/python-docs.yml)
[![codecov](https://codecov.io/gh/NLeSC-COMPAS/mrstat-toolkit/graph/badge.svg?token=4D7LUN3DU4)](https://codecov.io/gh/NLeSC-COMPAS/mrstat-toolkit)

[![julia-ci](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/julia-ci.yml/badge.svg?branch=main)](https://github.com/NLeSC-COMPAS/mrstat-toolkit/actions/workflows/julia-ci.yml)

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

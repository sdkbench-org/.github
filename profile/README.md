<p align="center">
  <img src="https://raw.githubusercontent.com/sdkbench-org/sdkbench/main/assets/avatar.png" alt="SDKBench logo" width="160" height="160">
</p>

<h1 align="center">SDKBench</h1>

<p align="center"><strong>Reproducible performance and correctness benchmarks for SDKs.</strong></p>

<p align="center">
  <a href="https://pypi.org/project/sdkbench/"><img src="https://img.shields.io/pypi/v/sdkbench" alt="PyPI version"></a>
  <a href="https://github.com/sdkbench-org/sdkbench"><img src="https://img.shields.io/badge/source-GitHub-181717?logo=github" alt="Source repository"></a>
  <a href="https://github.com/sdkbench-org/sdkbench/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-blue" alt="Project license: Apache-2.0"></a>
</p>

## About

SDKBench measures development-kit operations on shared, deterministic workloads and checks their outputs for correctness. The first release supports Qiskit and Cirq, with a NumPy reference adapter for validation and harness development.

面向开发套件的性能与正确性测评，首期接入 Qiskit 和 Cirq，提供统一电路、计时统计和结果校验。

## Install

```bash
pip install sdkbench

# Optional Qiskit and Cirq adapters
pip install 'sdkbench[all]'
```

## Try it

```bash
sdkbench list
sdkbench run --qubits 4 --output reference.json
sdkbench run --sdk qiskit --sdk cirq --output results.json --csv results.csv
```

## Available today

- Four deterministic circuit families: GHZ, QFT, brickwork and echo.
- Construction, inversion, composition, simulation and compilation benchmarks.
- Raw timing samples, correctness checks, JSON/CSV reports and matched-run comparisons.

The reference adapter works with the base install. The two-SDK command requires the optional adapters. These small, locally verifiable workloads do not constitute a comprehensive SDK ranking.

## Start here

- **[Source repository](https://github.com/sdkbench-org/sdkbench)** — implementation, examples and contributions.
- **[Documentation and quick start](https://github.com/sdkbench-org/sdkbench#readme)** — APIs, commands and methodology.
- **[PyPI package](https://pypi.org/project/sdkbench/)** — installation and release files.
- **[Issues and proposals](https://github.com/sdkbench-org/sdkbench/issues)** — bugs, new tasks and feature requests.

## Benchmark family

| Project | Focus | Package |
| --- | --- | --- |
| [LastExam](https://github.com/lastexam-org) | AI and agent task evaluation | [lastexam](https://pypi.org/project/lastexam/) |
| [SDKBench](https://github.com/sdkbench-org) | SDK performance and correctness | [sdkbench](https://pypi.org/project/sdkbench/) |
| [QCBench](https://github.com/qcbench-org) | Quantum computer hardware characterization | [qcbench](https://pypi.org/project/qcbench/) |

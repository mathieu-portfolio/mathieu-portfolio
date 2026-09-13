# Mathieu — Systems, HPC & Validation Engineer

I build performance-oriented software around systems programming, high-performance computing, data pipelines, and inference validation.

My projects focus on problems where correctness and performance both need to be observable: deterministic execution, numerical validation, profiling, concurrency, data movement, reproducible experiments, and measurable system behavior.

I prefer explicit architectures, controlled experiments, and implementations that make it possible to explain not just whether something works, but why it behaves the way it does.

---

## Featured Projects

### [sensor-platform](https://github.com/mathieu-portfolio/sensor-platform)

End-to-end C++20 and Python platform for multi-sensor simulation, event processing, tracking, transport, and analytical data pipelines.

A deterministic multi-radar source produces replayable observations that can be processed locally or through Kafka, fused into global tracks, inspected graphically, and transformed into validated Parquet datasets for SQL analysis.

* deterministic multi-radar event generation and replay
* typed event model with sequencing and lifecycle validation
* local and Kafka-based processing paths
* truth-free multi-sensor track fusion
* controlled load, backlog, outage, and recovery experiments
* incremental and idempotent raw-to-Parquet ingestion
* data-quality gates and conflict detection
* DuckDB/SQL analytical pipelines
* reproducible multi-seed experiments and performance studies
* graphical event and tracking visualization
* separation of runtime observations from offline ground-truth evaluation

Tech: C++20, Python, CMake, Kafka, Parquet, DuckDB, SQL, raylib

### [hpc-lab](https://github.com/mathieu-portfolio/hpc-lab)

Progressive high-performance computing laboratory built around matrix multiplication and numerical kernels.

The project follows a measurement-driven workflow: establish a correct baseline, benchmark it, identify a bottleneck, apply one optimization, and measure the result.

* naive and optimized GEMM implementations
* systematic loop-order experiments
* cache blocking and memory-locality analysis
* compiler auto-vectorization analysis
* generated assembly and disassembly inspection
* explicit AVX2/FMA SIMD kernels
* Roofline performance analysis
* OpenMP parallel implementations
* strong-scaling experiments
* thread affinity and NUMA investigations
* reproducible benchmark and reporting infrastructure

The longer-term progression includes packing, CUDA, MPI, sparse kernels, FFTs, and a consolidated benchmark suite.

Tech: C++20, CMake, OpenMP, AVX2/FMA, GCC/MSYS2, performance profiling

### [inference-validation-lab](https://github.com/mathieu-portfolio/inference-validation-lab)

Small inference-validation laboratory exploring how neural-network models can be exported, executed across runtimes, and checked systematically for numerical and structural correctness.

* deterministic test-input generation
* reference execution with PyTorch
* ONNX model export
* ONNX Runtime execution
* graph and export validation
* numerical comparison across inference backends
* dynamic batch-size validation
* reusable validation pipelines across MLP and CNN models
* automated regression tests for inference equivalence

The project is intentionally small and test-oriented, focusing on the workflow needed to diagnose model portability and runtime compatibility issues.

Tech: Python, PyTorch, ONNX, ONNX Runtime, pytest

### [particles3d-cuda](https://github.com/mathieu-portfolio/particles3d-cuda)

Interactive particle simulation exploring CPU and GPU execution scaling.

* CPU and CUDA simulation backends
* runtime-switchable execution modes
* GPU benchmarking infrastructure
* throughput and scaling experiments
* large-scale particle simulation
* runtime diagnostics and performance overlays

Tech: C++20, CUDA, CMake, raylib

### [memory-playground](https://github.com/mathieu-portfolio/memory-playground)

Interactive C++ environment for exploring memory locality and cache behavior.

* deterministic memory-hierarchy simulation
* cache-line loading and eviction
* structured instrumentation and traces
* timeline-based execution analysis
* reproducible benchmark scenarios
* cache-pressure and access-pattern visualization

Tech: C++20, CMake, raylib

### [cpp-systems-explorations](https://github.com/mathieu-portfolio/cpp-systems-explorations)

Focused systems-programming experiments covering low-level runtime components and execution models.

Topics include arena allocators, custom containers, thread pools, task graphs, and work-stealing schedulers.

Tech: C++, concurrency, memory management, runtime architecture

---

## Additional Projects

**Simulation & Tracking** — [sensor-sandbox](https://github.com/mathieu-portfolio/sensor-sandbox), the deterministic sensor-simulation core used by `sensor-platform`, with procedural targets, configurable radar behavior, uncertainty, noise, false positives, and tracking experiments.

**Large-Scale Simulation** — [flock3d](https://github.com/mathieu-portfolio/flock3d), a deterministic 3D boids simulation exploring spatial partitioning, fixed-timestep simulation, profiling, and scalability.

**Simulation Architecture** — [cpp-sim-lab](https://github.com/mathieu-portfolio/cpp-sim-lab), a collection of experiments around deterministic update pipelines, benchmarking, and parallel simulation architectures.

**Developer Tooling** — [job-intel](https://github.com/mathieu-portfolio/job-intel), a local-first job-analysis platform with configurable scoring and transparent evaluation.

Other repositories include procedural-generation experiments and earlier game-development projects.

---

## Engineering Approach

I tend to work from a simple, correct baseline and progressively introduce complexity only when measurements justify it.

That usually means:

* deterministic and reproducible inputs
* explicit invariants and ownership
* tests before optimization
* profiling before architectural changes
* controlled experiments instead of anecdotal benchmarks
* separation between runtime behavior and evaluation tooling
* recorded results that make regressions and trade-offs visible

I am particularly interested in the boundary between software architecture and hardware behavior: memory locality, vectorization, parallel execution, scheduling, data movement, accelerator runtimes, and numerical correctness.

---

## Currently

Focusing on C++ systems, HPC, and AI/inference validation roles.

Current areas of study and experimentation include:

* numerical and inference-runtime validation
* ONNX and heterogeneous inference pipelines
* SIMD and CPU microarchitecture
* OpenMP, NUMA, and parallel scaling
* CUDA and heterogeneous computing
* profiling and performance modeling
* reproducible data and benchmarking pipelines

---

## Contact

* Email: [mathieu.sterlin@gmail.com](mailto:mathieu.sterlin@gmail.com)
* LinkedIn: [mathieu-sterlin](https://www.linkedin.com/in/mathieu-sterlin-45300024b)

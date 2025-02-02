# LLVM Compilers on Polaris

This page is not about LLVM-based Cray Compiling Environment (CCE) compilers from `PrgEnv-cray` but about open source LLVM compilers.
If LLVM compilers are needed without MPI support, simply load the `llvm` or `llvm-sycl` module. 

Cray Programming Environment does not offer LLVM compiler support.
Thus cc/CC/ftn compiler wrappers using LLVM compilers currently are not available.
To use Clang with MPI, one can load the `mpiwrappers/cray-mpich-llvm` module which loads the following modules.

* `llvm`, upstream llvm compilers
* `cray-mpich`, MPI compiler wrappers mpicc/mpicxx/mpif90. mpif90 uses gfortran because flang is not ready for production use.
* `cray-pals`, MPI launchers mpiexec/aprun/mpirun


**Limitation** There is no GPU-aware MPI library linking support by default. If needed, users should manually add the GTL (GPU Transport Layer) library to the application link line.

[//]: # (ToDo: Lack of support for PrgEnv-cray is based on man page; should confirm)

## OpenMP offload

When targeting the OpenMP or CUDA programming models for GPUs, the `cudatoolkit-standalone` module should also be loaded.


[//]: # (ToDo: create examples and document)

## SYCL

For users working with the SYCL programming model, a separate `llvm` module can be loaded in the environment with support for the A100 GPUs on Polaris.

```
module load llvm-sycl/2022-06
```

[//]: # (ToDo: create examples and document)
[//]: # (ToDo: should get )

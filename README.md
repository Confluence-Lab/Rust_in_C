# Rust_in_C

The aim of this project is to study the effects of gradual introduction of Rust into a C++ codebase. We will be doing so through a case study of the gnss-sdr repository.

The preliminary plan is to start rustifying the signal processign blocks, and benchmarking the speed and memory leaks at different percentages of rustification of the codebase.

Plan for Testing and Benchmarking :

1)Static analysis to be done to detect memory errors using the tools rustc and Cppcheck.

2)Compare memory usage, speed, cpu usage using cargo-benchcmp for rust and google benchmark for C++. Verify the multithreading claims made by Rust.

3)Code size : Rust code can be compiled into smaller binaries which might be useful for small devices/iot. Compare binary sizes.

We will be making use of Rust ffi and the cxx-crate to integrate Rust into the codebase.

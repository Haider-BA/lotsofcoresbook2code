# Next Version
* Now using Markdown for README and CHANGELOG.
* Bugfix: example SVD now respects order of the passed matrices when applying the `dgemm` routine.
* Refactoring: simplified bridge between pyMIC and LIBXSTREAM.


# Version 0.5
* Introduced new kernel API that avoids insane pointer unpacking.
* pyMIC now uses _libxstreams_ as the offload back-end (<https://github.com/hfp/libxstream>).
* Added smart pointers to make handling of fake pointers easier.


# Version 0.4
* New low-level API to allocate, deallocate, and transfer data (see `OffloadStream`).
* Support for in-place binary operators.
* New internal design to handle offloads.


# Version 0.3
* Improved handling of libraries and kernel invocation.
* Trace collection (`PYMIC_TRACE=1`, `PYMIC_TRACE_STACKS={none,compact,full}`).
* Replaced the device-centric API with a stream API.
* Refactoring to better match PEP8 recommendations.
* Added support for `int` (`int64`) and `complex` (`complex128`) data types.
* Reworked the benchmarks and examples to fit the new API.
* Bugfix: fixed syntax errors in `OffloadArray`.


# Version 0.2
* Small improvements to the README files.
* New example: Singular Value Decomposition.
* Some documentation for the API functions.
* Added a basic testsuite for unit testing (WIP).
* Bugfix: benchmarks now use the latest interface.
* Bugfix: `numpy.ndarray` does not offer an attribute `order`.
* Bugfix: `number_of_devices` was not visible after import.
* Bugfix: member `offload_array.device` is now initialized.
* Bugfix: use exception for errors w/ `invoke_kernel` & `load_library`.


# Version 0.1
Initial release.

## Support Kokkos built with HIP as a CMake language

Viskores now builds with a Kokkos HIP backend that was compiled with HIP as a
CMake language (`Kokkos_ENABLE_COMPILE_AS_CMAKE_LANGUAGE`). The C++ compiler can
then be any host compiler, such as GCC, while the device sources are compiled by
the HIP compiler. When `CMAKE_HIP_ARCHITECTURES` is not set, Viskores now
compiles for the GPU architectures that Kokkos was built for.

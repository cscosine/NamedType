# NamedType: the cscosine copy

NamedType (strong types for C++, header-only: 5 headers, about 640 lines), as built and released by
[third_party_base_libs](https://github.com/cscosine/third_party_base_libs) for the cscosine projects. Kept as a
repository of our own: upstream has had no change since 2022.

| | |
|---|---|
| Came from | <https://github.com/joboccara/NamedType> |
| Base | upstream `master`, commit `76668ab` (2022-09-29, the last upstream commit; after the `v1.1.0` tag) |
| Our version | `1.1.0` (`project()` of `CMakeLists.txt`) |
| License | upstream's (`LICENSE`, MIT) |

## What we changed

- `CMakePresets.json`, `csCMakeProjectSetup.json`: built with the csCMake presets.
- The CMake package installed in `share/NamedType/cmake/` (instead of `lib/cmake/`: a header-only package).
- The tests use the Catch2 3 package of third_party_base_libs (`find_package(Catch2 3)`, `Catch2::Catch2WithMain`)
  instead of the `catch.hpp` of Catch2 1.x bundled upstream (15 000 lines, removed).

`git log 76668ab..dev` lists the commits.

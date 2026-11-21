# fmt-eigen: the cscosine copy

fmt-eigen (formatting of Eigen matrices with fmt: one header, about 100 lines), as built and released by
[third_party_base_libs](https://github.com/cscosine/third_party_base_libs) for the cscosine projects. Kept as a
repository of our own: upstream has no releases and no change since 2024.

| | |
|---|---|
| Came from | <https://github.com/RENyunfan/fmt-eigen> (author Yunfan REN) |
| Base | upstream `main`, commit `aa63bc0` (2024-11-24, "Update fmt_eigen.h"; no releases upstream) |
| Our version | `1.0.0` (`project()` of our `CMakeLists.txt`) |
| License | MIT, in the header (`fmt-eigen/fmt_eigen.h`, Copyright (c) 2024 Yunfan REN): keep that notice |

## What we changed

A csCMake project around the header: `fmt-eigen/fmt_eigen.h` (moved from the top folder), our `CMakeLists.txt`
(package `fmt-eigen`, depending on fmt and Eigen), `CMakePresets.json` and `csCMakeProjectSetup.json` (csCMake
presets), a sample (`sample/`); the IDE files of upstream (`.idea/`) removed. `git log aa63bc0..main` lists the commits.

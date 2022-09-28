Invoke with:
meson --native-file <src_path>/meson-vcpkg.txt --wrap-mode nodownload <src_path>

Will automatically invoke vcpkg to install dependencies listed in vcpkg.json

Example output:
```
The Meson build system
Version: 0.62.1
Source dir: E:\vcpkg_folders\meson_vcpkg
Build dir: E:\vcpkg_folders\meson_vcpkg\build
Build type: native build
Project name: meson-vcpkg
Project version: undefined
C++ compiler for the host machine: cl (msvc 19.33.31630 "Microsoft (R) C/C++-Optimierungscompiler Version 19.33.31630 f�r x64")
C++ linker for the host machine: link link 14.33.31630.0
Host machine cpu family: x86_64
Host machine cpu: x86_64
Program vcpkg found: YES
WARNING: You should add the boolean check kwarg to the run_command call.
         It currently defaults to false,
         but it will default to true in future releases of meson.
         See also: https://github.com/mesonbuild/meson/issues/9300
Found pkg-config: E:/vcpkg_folders/meson_vcpkg/vcpkg_installed/x64-windows/tools/pkgconf/pkgconf.exe (1.8.0)
Run-time dependency fmt found: YES 9.0.0
Run-time dependency zlib found: YES 1.2.12
Found CMake: C:\Program Files\CMake\bin\cmake.EXE (3.23.1)
Run-time dependency double-conversion found: YES 3.2.0
Build targets in project: 1
```
meson-log.txt will contain the installation information of vcpkg

Just for me:
G:\vcpkg_common\downloads\tools\python\python-3.10.5-x64\python  E:/vcpkg_folders/master_clean/installed/x64-windows/tools/meson/meson.py --native-file ../meson-vcpkg.txt --wrap-mode nodownload ../
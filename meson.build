project('meson-vcpkg', 'cpp',
    default_options: ['default_library=shared',
                      'cpp_std=c++latest'])

#would like to use variables from meson-vcpkg.txt here to refine
#the vcpkg call but meson won't let me do that.
vcpkg = find_program('vcpkg', required : true)
run_command(vcpkg, 'install', '--x-wait-for-lock',
                              '--x-manifest-root=' + meson.current_source_dir())

fmt_dep = dependency('fmt' ,  method : 'pkg-config')
zlib_dep = dependency('zlib')
double_conversion_dep = dependency('double-conversion')

executable('deptest', 'main.cpp',
   dependencies: [fmt_dep])
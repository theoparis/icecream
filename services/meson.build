inc = include_directories('.')

lzo2 = dependency('lzo2')
zstd = dependency('zstd', modules: ['zstd::libzstd_shared', 'zstd::libzstd_static'])

libicecc = library(
  'icecc',
  './comm.cpp',
  './exitcode.cpp',
  './gcc.cpp',
  './getifaddrs.cpp',
  './job.cpp',
  './logging.cpp',
  './pipes.cpp',
  './util.cpp',
  './platform.cpp',
  './tempfile.c',
  './ncpus.c',
  include_directories: [inc, configuration_inc],
  dependencies: [lzo2, zstd],
)

libicecc_dep = declare_dependency(link_with: libicecc, include_directories: inc)


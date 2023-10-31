libarchive = dependency('libarchive')
libcap = dependency('libcap-ng')

executable(
	'iceccd',
	'./main.cpp',
	'./serve.cpp',
	'./workit.cpp',
	'./environment.cpp',
	'./load.cpp',
	'./file_util.cpp',
	include_directories: [include_directories('.'), configuration_inc],
	dependencies: [libicecc_dep, libarchive, libcap],
)


inc = include_directories('.')

icecream_client = library(
	'icecream-client',
	'./arg.cpp',
	'./argv.c',
	'./cpp.cpp',
	'./local.cpp',
	'./remote.cpp',
	'./util.cpp',
	'./md5.c',
	'./safeguard.cpp',
	include_directories: [inc, configuration_inc],
	dependencies: [libicecc_dep],
  install: true,
)

icecream_client_dep = declare_dependency(link_with: icecream_client, include_directories: inc)

executable(
	'icecc',
	'./main.cpp',
	include_directories: [inc, configuration_inc],
	dependencies: [libicecc_dep, icecream_client_dep],
  install: true,
)


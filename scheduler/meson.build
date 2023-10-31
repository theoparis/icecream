executable(
	'icecc-scheduler',
	'./compileserver.cpp',
	'./job.cpp',
	'./jobstat.cpp',
	'./scheduler.cpp',
	include_directories: [
		include_directories('.'),
		configuration_inc,
	],
	dependencies: [libicecc_dep],
)


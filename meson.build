project('lzham', 'cpp')

add_project_arguments(
	'-D_WIN32_WINNT=0x0601',
	'-DWINVER=0x0601',
	'-DWIN32',
	language: [ 'cpp', 'c' ]
)

include_dir = include_directories('include')

subdir('lzhamdecomp')
subdir('lzhamcomp')
subdir('lzhamlib')

lzham_dep = declare_dependency(
	include_directories: include_dir,
	dependencies: [
		lzhamcomp_dep,
		lzhamdecomp_dep,
		lzhamlib_dep,
	]
)
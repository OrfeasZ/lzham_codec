lzhamlib_src = [
	'lzham_lib.cpp',
]

# Targets.
lzhamlib = static_library('lzhamlib',
	lzhamlib_src,
	include_directories: [ include_directories('.'), include_dir ],
	dependencies: [ lzhamcomp_dep ]
)

lzhamlib_dep = declare_dependency(
	link_with: lzhamlib,
	include_directories: [ include_directories('.') ],
	dependencies: [ lzhamcomp_dep ]
)
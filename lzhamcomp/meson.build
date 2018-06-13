lzhamcomp_src = [
	'lzham_lzbase.cpp',
	'lzham_lzcomp.cpp',
	'lzham_lzcomp_internal.cpp',
	'lzham_lzcomp_state.cpp',
	'lzham_match_accel.cpp',
	#'lzham_pthreads_threading.cpp',
	'lzham_win32_threading.cpp',
]

# TODO: If linux add pthreads

# Targets.
lzhamcomp = static_library('lzhamcomp',
	lzhamcomp_src,
	include_directories: [ include_directories('.'), include_dir ],
	dependencies: [ lzhamdecomp_dep ]
)

lzhamcomp_dep = declare_dependency(
	link_with: lzhamcomp,
	include_directories: [ include_directories('.') ],
	dependencies: [ lzhamdecomp_dep ]
)
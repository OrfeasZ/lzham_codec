lzhamdecomp_src = [
	'lzham_assert.cpp',
	'lzham_checksum.cpp',
	'lzham_huffman_codes.cpp',
	'lzham_lzdecomp.cpp',
	'lzham_lzdecompbase.cpp',
	'lzham_mem.cpp',
	'lzham_platform.cpp',
	'lzham_prefix_coding.cpp',
	'lzham_symbol_codec.cpp',
	'lzham_timer.cpp',
	'lzham_vector.cpp',
]

# Targets.
lzhamdecomp = static_library('lzhamdecomp',
	lzhamdecomp_src,
	include_directories: [ include_directories('.'), include_dir ],
)

lzhamdecomp_dep = declare_dependency(
	link_with: lzhamdecomp,
	include_directories: [ include_directories('.') ],
)
project(
	'vulkan-playground',
	'c',
	default_options: 'default_library=static'
)

cmake = import('cmake')

# VULKAN
vulkan_dep = dependency('vulkan')

# CGLM
cglm_dep = dependency('cglm')

# SDL2
sdl2_dep = dependency('sdl2')
sdl2_main_dep = dependency('sdl2main')

src = files(
	'src/main.c'
)

executable(
	'vulkan-playground',
	src,
	win_subsystem: 'windows',
	dependencies: [
		cglm_dep,
		sdl2_dep,
		sdl2_main_dep
	]
)
project(
	'vulkan-playground',
	'c',
	default_options: 'default_library=static'
)

cglm_dep = dependency('cglm')
glfw_dep = dependency('glfw3')

src = files(
	'src/main.c'
)

executable('vulkan-playground', src, win_subsystem: 'windows', dependencies: [cglm_dep, glfw_dep])
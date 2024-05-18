project(
	'vulkan-playground',
	'c',
	default_options: 'default_library=static'
)

cmake = import('cmake')

# CGLM
cglm_dep = dependency('cglm')

# GLFW
glfw_proj = cmake.subproject('glfw')
glfw_dep = glfw_proj.dependency('glfw')

src = files(
	'src/main.c'
)

executable('vulkan-playground', src, win_subsystem: 'windows', dependencies: [cglm_dep, glfw_dep])
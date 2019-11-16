project(fosl-arm-util)

add_library(
	${PROJECT_NAME}

	./fosl/arm/util.h
	./fosl/arm/util.cpp
)

target_include_directories(
	${PROJECT_NAME} PUBLIC

	${PROJECT_SOURCE_DIR}

	${fosl-math_SOURCE_DIR}
	${fosl-util_SOURCE_DIR}
)

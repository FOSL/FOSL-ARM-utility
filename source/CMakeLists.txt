project(fosl-arm-util)

add_library(
	${PROJECT_NAME}

	./fosl/arm/util.cpp
	./fosl/arm/util.h
)

target_include_directories(
	${PROJECT_NAME} PUBLIC

	${PROJECT_SOURCE_DIR}
	${fosl-util_SOURCE_DIR}
)

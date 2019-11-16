project(fosl-arm-util)

add_library(
	${PROJECT_NAME}

	./util/assert.h
	./util/bits.h
	./util.cpp
	./util.h
)

target_include_directories(
	${PROJECT_NAME} PUBLIC

	${PROJECT_SOURCE_DIR}
	${math_SOURCE_DIR}
)

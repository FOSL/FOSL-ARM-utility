project(FOSL-ARM-utility)

add_library(
	${PROJECT_NAME}

	./FOSL/ARM/utility.hpp
	./FOSL/ARM/utility.cpp
)

target_include_directories(
	${PROJECT_NAME} PUBLIC

	${PROJECT_SOURCE_DIR}
)

target_link_libraries(
	${PROJECT_NAME}

	FOSL-utility
)

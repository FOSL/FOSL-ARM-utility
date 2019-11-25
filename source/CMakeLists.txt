project(FOSL-ARM-Utilities)

add_library(
	${PROJECT_NAME}

	./FOSL/ARM/Utilities.hpp
	./FOSL/ARM/Utilities.cpp
)

target_include_directories(
	${PROJECT_NAME} PUBLIC

	${PROJECT_SOURCE_DIR}
)

target_link_libraries(
	${PROJECT_NAME}

	FOSL-Utilities
)

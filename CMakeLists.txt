# CMakeLists files in this project can
# refer to the root source directory of the project as ${HELLO_SOURCE_DIR} and
# to the root binary directory of the project as ${HELLO_BINARY_DIR}.
cmake_minimum_required (VERSION 2.8.11)
project (MeshFix)
add_definitions(-DIS64BITPLATFORM)

# Recurse into the "Hello" and "Demo" subdirectories. This does not actually
# cause another cmake executable to run. The same process will walk through
# the project's entire directory structure.
add_subdirectory (src/Algorithms)
add_subdirectory (src/TMesh)
add_subdirectory (src/Kernel)
add_subdirectory (src/MeshFix)


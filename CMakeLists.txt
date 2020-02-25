cmake_minimum_required(VERSION 3.12)
project(py-packaging VERSION 0.1.0)

include(GNUInstallDirs)

find_package(Python REQUIRED Interpreter Development)

# PyBind11
# NB: Need to worry about the handling of C++ standard flags here
# See pybind11 docs and the PYBIND11_CPP_STANDARD variable
add_subdirectory(pybind11)

# The C++ library
#add_library()

# The Python binding
#python_add_library() or pybind11_add_module()?

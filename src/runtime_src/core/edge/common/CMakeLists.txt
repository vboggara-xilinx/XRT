# SPDX-License-Identifier: Apache-2.0
# Copyright (C) 2019-2021 Xilinx, Inc. All rights reserved.
#
include_directories(
  ${CMAKE_CURRENT_SOURCE_DIR}
  ${Boost_INCLUDE_DIRS}
  ${CMAKE_BINARY_DIR} # version.h
  )

file(GLOB EDGE_COMMON_OBJ_FILES "*.cpp")
add_library(core_edge_common_objects OBJECT ${EDGE_COMMON_OBJ_FILES})

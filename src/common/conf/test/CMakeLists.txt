# Copyright (c) 2020 vesoft inc. All rights reserved.
#
# This source code is licensed under Apache 2.0 License.

nebula_add_test(
    NAME configuration_test
    SOURCES ConfigurationTest.cpp
    OBJECTS $<TARGET_OBJECTS:conf_obj> $<TARGET_OBJECTS:fs_obj> $<TARGET_OBJECTS:base_obj>
    LIBRARIES gtest gtest_main
)

add_executable(boost_test_integration main.cpp)
target_link_libraries(boost_test_integration rapidcheck_boost_test boost)
if (MSVC)
  target_compile_options(boost_test_integration PRIVATE "/EHa")
endif()

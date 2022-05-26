add_executable(slsqp_test_exe)
target_sources(slsqp_test_exe PRIVATE slsqp_test.f90)
target_link_libraries(slsqp_test_exe PRIVATE ${PROJECT_NAME})
add_test(NAME slsqp_test COMMAND slsqp_test_exe)

add_executable(slsqp_test_2_exe)
target_sources(slsqp_test_2_exe PRIVATE slsqp_test_2.f90)
target_link_libraries(slsqp_test_2_exe PRIVATE ${PROJECT_NAME})
add_test(NAME slsqp_test_2 COMMAND slsqp_test_2_exe)

add_executable(slsqp_test_3_exe)
target_sources(slsqp_test_3_exe PRIVATE slsqp_test_3.f90)
target_link_libraries(slsqp_test_3_exe PRIVATE ${PROJECT_NAME})
add_test(NAME slsqp_test_3 COMMAND slsqp_test_3_exe)

add_executable(slsqp_test_stopping_criterion_exe)
target_sources(slsqp_test_stopping_criterion_exe PRIVATE
  slsqp_test_stopping_criterion.f90)
target_link_libraries(slsqp_test_stopping_criterion_exe PRIVATE ${PROJECT_NAME})
add_test(NAME slsqp_test_stopping_criterion COMMAND slsqp_test_stopping_criterion_exe)

add_executable(slsqp_test_71_exe)
target_sources(slsqp_test_71_exe PRIVATE slsqp_test_71.f90)
target_link_libraries(slsqp_test_71_exe PRIVATE ${PROJECT_NAME})
add_test(NAME slsqp_test_71 COMMAND slsqp_test_71_exe)

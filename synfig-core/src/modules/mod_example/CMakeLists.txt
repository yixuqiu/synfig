add_library(mod_example MODULE
        "${CMAKE_CURRENT_LIST_DIR}/main.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/metaballs.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/simplecircle.cpp"
)

target_link_libraries(mod_example libsynfig)

install (
    TARGETS mod_example
    DESTINATION lib/synfig/modules
)

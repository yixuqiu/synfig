add_library(mod_dv MODULE
        "${CMAKE_CURRENT_LIST_DIR}/main.cpp"
        "${CMAKE_CURRENT_LIST_DIR}/trgt_dv.cpp"
)

target_link_libraries(mod_dv libsynfig)

install (
    TARGETS mod_dv
    DESTINATION lib/synfig/modules
)

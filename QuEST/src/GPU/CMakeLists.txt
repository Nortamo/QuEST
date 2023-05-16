
if (AMD_GPU)
    set(QuEST_SRC_ARCHITECTURE_DEPENDENT
        ${CMAKE_CURRENT_SOURCE_DIR}/QuEST_gpu.hip.cu
        PARENT_SCOPE
    )
else()
    set(QuEST_SRC_ARCHITECTURE_DEPENDENT
        ${CMAKE_CURRENT_SOURCE_DIR}/QuEST_gpu.cu
        PARENT_SCOPE
    )
endif()


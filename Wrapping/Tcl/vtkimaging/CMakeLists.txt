IF(NOT VTK_INSTALL_NO_RUNTIME)

  CONFIGURE_FILE(
    ${CMAKE_CURRENT_SOURCE_DIR}/vtkimaging.tcl.in
    ${CMAKE_CURRENT_BINARY_DIR}/vtkimaging.tcl
    @ONLY)

  INSTALL(FILES
    ${CMAKE_CURRENT_BINARY_DIR}/vtkimaging.tcl
    DESTINATION ${VTK_TCL_INSTALL_DIR_CM24}/vtkimaging
    COMPONENT RuntimeLibraries)
ENDIF(NOT VTK_INSTALL_NO_RUNTIME)

# CMakeLists.txt at root
set(COMPONENT_SRCS
    "components/Sensors/sensor.c"
    "components/Display/display.c"
)

set(COMPONENT_ADD_INCLUDEDIRS
    "components/Sensors"
    "components/Display"
)

# Register all components in this directory
idf_component_register(
    SRCS ${COMPONENT_SRCS}
    INCLUDE_DIRS ${COMPONENT_ADD_INCLUDEDIRS}
)


message(INFO "<MS>")
message(INFO "<MS> BHY2-Sensor-API >>")
message(INFO "<MS>")
message(INFO "<MS> CMAKE_CURRENT_SOURCE_DIR: ${CMAKE_CURRENT_SOURCE_DIR}")


set(BHY2_Sensor_API_SRCS 
    bhy2_hif.c
    bhy2.c
    bhy2_parse.c
    )
set(BHY2_Sensor_API_INCL ${CMAKE_CURRENT_SOURCE_DIR})
set(BHY2_Sensor_API_REQU )

idf_component_register(
    INCLUDE_DIRS ${BHY2_Sensor_API_INCL} 
    SRCS ${BHY2_Sensor_API_SRCS}
    REQUIRES ${BHY2_Sensor_API_REQU}
    )

message(INFO "<MS>")
message(INFO "<MS> BHY2-Sensor-API <<")
message(INFO "<MS>")

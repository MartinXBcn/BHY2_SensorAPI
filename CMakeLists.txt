
set(BHY2_SensorAPI_SRCS 
    bhy2_hif.c
    bhy2.c
    bhy2_parse.c
    )
set(BHY2_SensorAPI_INCL ${CMAKE_CURRENT_SOURCE_DIR})
set(BHY2_SensorAPI_REQU )

idf_component_register(
    INCLUDE_DIRS ${BHY2_SensorAPI_INCL} 
    SRCS ${BHY2_SensorAPI_SRCS}
    REQUIRES ${BHY2_SensorAPI_REQU}
    )


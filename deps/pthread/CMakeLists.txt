CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(TDengine)

IF (TD_WINDOWS_64 OR TD_WINDOWS_32)
  INCLUDE_DIRECTORIES(.)
  LIST(APPEND SRC pthread.c)
  ADD_LIBRARY(pthread ${SRC})
ENDIF ()

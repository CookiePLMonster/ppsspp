set(SRCS
  lin/matrix4x4.cpp
  lin/vec3.cpp
  lin/quat.cpp
	curves.cpp
	math_util.cpp
  )

set(SRCS ${SRCS})

add_library(lin STATIC ${SRCS})

if(UNIX)
  add_definitions(-fPIC)
endif(UNIX)

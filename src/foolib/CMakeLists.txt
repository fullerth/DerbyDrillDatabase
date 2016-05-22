set (FOOLIB_SOURCES
     foo.cpp)

include_directories(foolib
	"include"
	)

add_library(foolib STATIC
	${FOOLIB_SOURCES}
	)

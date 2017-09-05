set(FILES
	 test.h)

list(APPEND FILES test.cpp)


add_library(test ${FILES})
#set_target_properties(ethash PROPERTIES C_STANDARD 99)
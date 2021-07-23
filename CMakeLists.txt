cmake_minimum_required (VERSION 3.8)
project (ue4-recast-detour C CXX)

file(GLOB_RECURSE DIR_SRCS Detour/*.cpp Detour/*.h Detour/*.hpp 
	ue4-detour.cpp ue4-findpath.cpp UE4RecastHelper.cpp UE4RecastHelper.h)
	
add_library(recast-detour ${DIR_SRCS})


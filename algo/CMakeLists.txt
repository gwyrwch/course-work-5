cmake_minimum_required(VERSION 3.14)
project(algo)

set(CMAKE_CXX_STANDARD 17)

set(SOURCE_LIB ISolution.cpp
        NearestNeighbour.cpp Test.cpp Tour.cpp Distance.cpp MinimumSpanningTree.cpp NaiveSolution.cpp
        LocalSearch.cpp IOptimizer.cpp BranchAndBound.cpp GeneticAlgorithm.cpp SimulatedAnnealing.cpp)

#add_subdirectory(a)
#add_subdirectory(b)

add_library(algo STATIC ${SOURCE_LIB})
target_link_libraries(algo util)

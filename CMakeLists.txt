cmake_minimum_required(VERSION 3.10)
project(Gist)
set(CMAKE_CXX_STANDARD 14)

include_directories(src)
set(SOURCE_FILES src/Gist.cpp
                 src/core/CoreFrequencyDomainFeatures.cpp
                 src/core/CoreTimeDomainFeatures.cpp
                 src/fft/AccelerateFFT.cpp
                 src/fft/WindowFunctions.cpp
                 src/mfcc/MFCC.cpp
                 src/onset-detection-functions/OnsetDetectionFunction.cpp
                 src/pitch/Yin.cpp)

add_library(Gist ${SOURCE_FILES})
cmake_minimum_required(VERSION 3.13)

set(PROJECT_NAME cmake_project_example) # set명령 : 변수 생성
set(CMAKE_CXX_STANDARD 17)  # pre-defined변수 : C++ 버전 17으로 설정

project(${PROJECT_NAME})    # 프로젝트 세팅 시작
add_executable(${PROJECT_NAME} src/main.cpp)    # 해당 cpp파일 컴파일해서 해당 이름으로 실행파일 생성

# 터미널명령: cmake -Bbuild . -DCMAKE_BUILD_TYPE=Debug   # [Debug|Release]
# 터미널명령: cmake --build build --config Debug
# 터미널명령: .\build\Debug\cmake_project_example.exe
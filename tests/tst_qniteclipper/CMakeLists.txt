find_package(
    Qt5
COMPONENTS
    Test
REQUIRED
)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_INCLUDE_CURRENT_DIR ON)

add_executable(
    tst_qniteclipper
    tst_qniteclipper.cpp
)

target_link_libraries(
    tst_qniteclipper
PRIVATE
    qnite
    Qt5::Test
)

add_test(
    tst_qniteclipper
    tst_qniteclipper
)

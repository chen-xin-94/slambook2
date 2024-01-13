## Sophus
https://blog.csdn.net/weixin_44120025/article/details/122244849

    在cMakeLists.txt中添加
    set(CMAKE_CXX_FLAGS "-Wno-error=deprecated-declarations -Wno-deprecated-declarations ")

## Ceres
https://blog.csdn.net/m0_56140527/article/details/132399507

sudo make install

## g2o
set eigen3 version to 3.2.5 

    直接更改了 cmake_modules/FindEigen3.cmake
    加了三行
    set(EIGEN3_FOUND TRUE)
    set(EIGEN3_INCLUDE_DIR,/usr/include/eigen3.2.5/include/eigen3)
    set(EIGEN3_VERSION "3.2.5")

built with lots of warnings

sudo make install
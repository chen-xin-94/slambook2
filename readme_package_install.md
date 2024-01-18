## eigen
sudo apt install 了 3.4版本
后手动安装了3.2.5版本，以适配ceres和g2o

## Sophus
https://blog.csdn.net/weixin_44120025/article/details/122244849

    在Sophus目录下，打开CMakeLists.txt文件，在里面加上如下一行代码（不加的话在make的时候会报错）:
    set(CMAKE_CXX_FLAGS "-Wno-error=deprecated-declarations -Wno-deprecated-declarations ")

sudo make install (only after ch12)

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

## opencv
安装了4.8版本
部分参考 https://github.com/Offliners/Slambook24Win 解决了其中列出的“error： 'xxxxxxx' was not declared in this scope”

## DBoW3
sudo make install
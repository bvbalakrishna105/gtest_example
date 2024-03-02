# gtest_example

# How to setup google test frame work for c++ code

First download the gtest repo

git clone https://github.com/google/googletest.git


Navigate the googletest directory

cd googletest

create a build  directory

mkdir build
cd build


Run  Cmake to generate the build files

cmake ..

Build gtest

make


For accessing the .a files through the system wide

sudo make install

Create a new folder and copy the test.cpp content for your testing

compile the code

vidkrix@venky-worker:~/Desktop/work/gtest_example$ g++ -o test test.cpp -I/home/vidkrix/Desktop/work/googletest/googletest/include/ -lgtest

run the test binary

vidkrix@venky-worker:~/Desktop/work/gtest_example$ ./test

[==========] Running 2 tests from 1 test suite.

[----------] Global test environment set-up.

[----------] 2 tests from AddTest

[ RUN      ] AddTest.PositiveNumbers

[       OK ] AddTest.PositiveNumbers (0 ms)

[ RUN      ] AddTest.NegativeNumbers

[       OK ] AddTest.NegativeNumbers (0 ms)

[----------] 2 tests from AddTest (0 ms total)

[----------] Global test environment tear-down

[==========] 2 tests from 1 test suite ran. (0 ms total)

[  PASSED  ] 2 tests.

vidkrix@venky-worker:~/Desktop/work/gtest_example$
cmake_minimum_required(VERSION 3.1)

project(acsdkStartupManagerInterfaces LANGUAGES CXX)

add_library(acsdkStartupManagerInterfaces INTERFACE)

target_include_directories(acsdkStartupManagerInterfaces INTERFACE
    "${acsdkStartupManagerInterfaces_SOURCE_DIR}/include")

target_link_libraries(acsdkStartupManagerInterfaces INTERFACE
    acsdkNotifierInterfaces)

# install interface
asdk_install_interface()

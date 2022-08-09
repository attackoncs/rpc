# set(SRC_LIST userservice.cc ../user.pb.cc)
set(SRC_LIST calluserservice.cc ../user.pb.cc)

add_executable(consumer ${SRC_LIST})
target_link_libraries(consumer mprpc protobuf)
#aux_source_directory(. SRC_LIST)
set(SRC_LIST 
    mprpcapplication.cc 
    rpcprovider.cc 
    mprpcconfig.cc
    rpcheader.pb.cc 
    )
# muduo是静态库，因此这里也生成静态库
add_library(mprpc ${SRC_LIST})
target_link_libraries(mprpc  muduo_net muduo_base  pthread)
#aux_source_directory(. SRC_LIST)
set(SRC_LIST 
    mprpcapplication.cc 
    rpcprovider.cc 
    mprpcconfig.cc
    )
add_library(mprpc ${SRC_LIST})
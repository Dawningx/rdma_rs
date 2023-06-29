编译选项：gcc rdma-new-client(server).c -lrdmacm -libverbs -lpthread -o client(server)

client运行方式：./client {ip} {port} {data}

server运行方式：./server

**PS:** 目前我做的server的运行逻辑是收到内容后第一个byte加1，比如收到'1'传回'2'，收到'a'传回'b'这种。后面可以针对报文格式做一个分析的代码。
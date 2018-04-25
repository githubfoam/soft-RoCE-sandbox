# soft-RoCE-sandbox
How to configure Soft-RoCE with Mellanox OFED-4.3 (work under progress)


HowTo Configure Soft-RoCE (Method 1: Inbox Driver)  
https://community.mellanox.com/docs/DOC-2184

How to configure Soft-RoCE with Mellanox OFED 4.2. (Method 2: Mellanox OFED Linux Driver)
https://community.mellanox.com/community/support/software-drivers/mellanox-ofed/blog/2017/12/22/how-to-configure-soft-roce-with-mellanox-ofed-42


The following are the supported OSs in MLNX_OFED Rev 4.2-1.0.0.0: 
Kernels 4.10-4.13 x86_64 
http://www.mellanox.com/related-docs/prod_software/Mellanox_OFED_Linux_Release_Notes_4_2-1_0_0_0.pdf

The following are the supported OSs in MLNX_OFED Rev 4.3-1.0.1.0
Kernels 4.14-4.15  x86_64
http://www.mellanox.com/related-docs/prod_software/Mellanox_OFED_Linux_Release_Notes_4_3-1_0_1_0.pdf

How-To Dump RDMA traffic Using the Inbox tcpdump tool (ConnectX-4)
https://community.mellanox.com/docs/DOC-2416

To verify RXE kernel module is loaded. Mellanox OFED-4.3

# lsmod |grep rdma_rxe 
rdma_rxe              114688  0 
ip6_udp_tunnel         16384  1 rdma_rxe 
udp_tunnel             16384  1 rdma_rxe 
ib_core               208896  9 rdma_rxe,ib_cm,rdma_cm,ib_umad,ib_uverbs,ib_ipoib,iw_cm,ib_ucm,rdma_ucm 
https://community.mellanox.com/docs/DOC-2184 
    
Validate that RXE is working
https://github.com/SoftRoCE/rxe-dev/wiki/Validate-that-RXE-is-working

RXE Test plan
https://github.com/SoftRoCE/rxe-dev/wiki/RXE-Test-plan


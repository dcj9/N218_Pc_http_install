# Create PXE Fedora 39 Server VM for N218 Clusters

- _https://docs.fedoraproject.org/en-US/fedora/f36/install-guide/advanced/Network_based_Installations/_

#updated 6/14/2024
5/29/2024

Setting up the fedora VM first on Chile
<pre><font color="#00AA00">csmone@chile</font>:<font color="#00AA00">~</font>$ ifconfig
enp0s31f6: flags=4163&lt;UP,BROADCAST,RUNNING,MULTICAST&gt;  mtu 1500
        inet 132.177.5.102  netmask 255.255.252.0  broadcast 132.177.7.255
        inet6 2606:4100:38c0:4::5:102  prefixlen 64  scopeid 0x0&lt;global&gt;
        inet6 fe80::83b9:d6d9:98d8:86cb  prefixlen 64  scopeid 0x20&lt;link&gt;
        ether b0:4f:13:14:4d:dd  txqueuelen 1000  (Ethernet)
        RX packets 354746  bytes 358074999 (341.4 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 42316  bytes 4308382 (4.1 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0
        device interrupt 16  memory 0x72280000-722a0000  

lo: flags=73&lt;UP,LOOPBACK,RUNNING&gt;  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10&lt;host&gt;
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 3596  bytes 445969 (435.5 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 3596  bytes 445969 (435.5 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

</pre>

<pre><font color="#00AA00">csmone@chile</font>:<font color="#00AA00">~</font>$ uname -a
Linux chile.cs.unh.edu 6.8.11-200.fc39.x86_64 #1 SMP PREEMPT_DYNAMIC Sun May 26 20:05:41 UTC 2024 x86_64 GNU/Linux
</pre>


# *Download mirrors for Fedora 39*
_https://www.server-world.info/en/note?os=Fedora_39&p=download_


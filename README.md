## Testing IPSec with netkit

[Netkit](http://wiki.netkit.org/) is the "poor man's system to experiment computer networking". Uning User-mode Linux it allows to simultate complex networks.

This setup test IPSec between 2 PC using ESP un AH on a network with a setup like the following:

PC1 <------->Router1<-------->Router2<-------->PC2

## How to run it
Download NetKit from:
http://wiki.netkit.org/index.php/Download_Official

    tar -xjSf netkit-x.y.tar.bz2
    tar -xjSf netkit-filesystem-Fx.y.tar.bz2
    tar -xjSf netkit-kernel-Kx.y.tar.bz2
    export NETKIT_HOME=$PWD/netkit
    export MANPATH=:$NETKIT_HOME/man
    export PATH=$NETKIT_HOME/bin:$PATH

    git clone https://github.com/nscendoni/netkit-ipsec.git
    cd netkit-ipsec
    lstart


## References
[IPSEC](http://www.tldp.org/HOWTO/VPN-HOWTO)

[NetKit](http://wiki.netkit.org/index.php/Labs_Official)

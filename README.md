# Config to bypass CGNAT using a VPS

These configs can be used to create a VPN to your local network via a middle hop hosted on a VPS (or other server solution).
I am using a Raspberry Pi 2 (running Raspbian) on my local network as an ingress point. The VPS is running Ubuntu. 

In this config the VPS sits in the middle and both the home network (Raspberry Pi) and client (phone or laptop) connect to the VPS in public IP space. This is to avoid the restrictions that carrier grage NAT places on my ability to tunnel back into my home network from an IPv4 only connection. 

IPv6 is working great at home and if I have IPv6 connectivty it is preferred as I can connect straight home rather than through an antermediate hop.

To-Do: I now have this setup able to tunnel IPv6 over the IPv4 connection, I need to update the config files here to reflect this enhancement.

Original Reddit post with more details here: https://www.reddit.com/r/WireGuard/comments/duif1e/my_config_for_bypassing_cgnat_with_vps/

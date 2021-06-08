# profinet-python
Minimal Profinet implementation in Python

https://github.com/devkid/profinet/issues/1#issuecomment-228459971

It basically contains a command line interface (main.py) and a web GUI (server.py) that can be used independently; 

you should be able to run the web server with 

python server.py -i eth0 

(or whatever NIC you are using). 

protocol.py contains the description of the different profinet packet types; 

dcp.py and rpc.py contain the implementation for the DCP and RPC privimites, respectively. 

I think you need to consult the profinet documentation to find out what exactly they are used for.

- gira su python3
- posso lanciare un discovery (_sudo python3 main.py discover -i enp4s0f0_)
- posso lanciarlo anche su PLCnext ma richiede utente root (_root@axcf1152:/opt/plcnext/profinet-python# python3 main.py discover -i eth0_)

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
- ho dovuto installare pip3 (_sudo apt install python3-venv python3-pip_)
- ho dovuto installare flask (_sudo pip3 install flask_)
- _sudo python3 main.py discover -i enp4s0f0 _

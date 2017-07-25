Install: 
- Download and Install Python 2.7.13 at: https://www.python.org/downloads/release/python-2713/
- Open file hosts at "C:\Windows\System32\drivers\etc\hosts" and add a line:

127.0.0.1 claymore-nofee.com

- Edit the file "start.bat" that runs Claymore to mine the pool at "claymore-nofee.com" and enable 0 for -esm (Ethereum Stratum mode). Remember to replace 0x27e1fbfe2d17f58a7f02166ceff6b7f99ede87de by your wallet address 

EthDcrMiner64.exe -epool claymore-nofee.com:8008 -ewal 0x27e1fbfe2d17f58a7f02166ceff6b7f99ede87de.rig2/test@gmail.com -epsw x -mode 1 -ftime 10 -esm 0 -lidag 1

- Edit "start-nofee.bat" by the following command:
nofee.pyo 127.0.0.1 8008 [your_mining_pool_ip] [your_mining_pool_ip] [your_wallet_address]

FOR EXAMPLE: nofee.pyo 127.0.0.1 8008 eth-us-west1.nanopool.org 9999 0x27e1fbfe2d17f58a7f02166ceff6b7f99ede87de

- Run "start-nofee.bat"
- Run file start.bat of Claymore
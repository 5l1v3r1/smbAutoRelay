## SMB AutoRelay
  SMB AutoRelay provides the automation of SMB/NTLM Relay technique for pentesting and red teaming exercises in active directory environments.
  
  
  **DISCLAIMER**: I AM NOT RESPONSIBLE OF THE MISUSE OF THIS TOOL. YOU RUN IT AT YOUR OWN RISK. PLEASE BE KIND :)
  
  Before running the tool, make sure you are in a controlled environment, and where you are allowed to perform this kind of exercise.

## Usage
  Syntax: `./smbAutoRelay.sh -i <interface> -t <pathToTargetsFile>`. 
  
  Example: `./smbAutoRelay.sh -i eth0 -t ./targets.txt`.
  
  > Notice that the targets file should contain just the IP addresses of each target, one per line, to which you want to try the SMB/NTLM Relay technique.
  
  To unninstall the software installed by the tool: `./smbAutoRelay.sh -r`.
  
  Run `./smbAutoRelay.sh [-h]` to open the help menu.
  
##

  **Software which it installs in the pwd [*needed to run properly*]**
  - responder
  - ntlmrelayx.py
  
  **Software which it installs through `apt` if not installed [*needed to run properly*]**
  - tmux
  - rlwrap
  - python
  - python3
  - netcat
  
## TODOs
  - [ ] Add the possibility to capture and crack the NetNTLM hash.
  - [ ] Fix weird issues

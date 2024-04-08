## Tor VPN  *PIF PEONEI* Changer

PIF-PEONEI script allows you to change your IP address using the Tor network. It runs a VPN session that changes the IP address at regular intervals that you specify.

## Features 
- **Starting the Tor Service:** Initiates the Tor service to establish a connection with the Tor network.
- **Change IP Address:** Updates the IP address using the Tor network.
- **Run VPN Session:** Initiates a VPN session with customizable duration and time interval between IP changes.
- **Show Contact Information:** Displays contact details for support. It also saves the IP address you used in a file named temp_ip.txt.

- **Fixes:**

Fixed code runtime issues.
Additions:

-1 Added `random.shuffle()`to the code to generate a random list of countries.
-2 Added `generate_countries_list:` A function to generate a random list of countries.
Here's a more detailed explanation of the changes:

Fixes:

- The original code had some runtime issues, such as not being able to find available ports or failing to start the Tor service. These issues have been fixed in the updated code.
Additions:

- The original code generated a fixed list of countries. The updated code uses the  `random.shuffle()`function to generate a random list of countries, making it more difficult to track the user's location.
- The updated code includes a new function called`generate_countries_list.`This function generates a random list of countries from a predefined list of continents. 
- This makes it easier to customize the list of countries used by the script.

## Dependencies

- Python 3.x
- `stem` library
- `colorama` library                            
- `random2`library
- `logging4` library
- `stem`library
- `colorama` library
- `socket`library

## Do you need the tor package to run this. Instal tor first!
> DEBIAN:
              
          apt update && apt upgrade && apt install tor torsocks -y
> GENTOO: 
       
          emerge tor torsocks

> ARCH: 
          
         pacman tor torsocks -Syu

> OPENSUSE: 
          
   
         zypper install tor torsocks -y `

## Install repositories Kali Linux


    git clone https://github.com/Mohamed9x60/TorVpn.git
    cd TorVpn
    pip install -r requirements.txt
    sudo python3 PIF-PEONEI.py
    
    


## Install repositories on Termux

    git clone https://github.com/Mohamed9x60/TorVpn.git
    cd TorVpn
    pip install -r requirements.txt
    python3 PIF-PEONEI.py
    


## Known Issues and Fixes

1. **OSError: Failed to start Tor service: reached  
'' the specified seconds'' timeout without success**: This error occurs when the script fails to start the Tor service within the specified timeout period. Check your internet connection, firewall settings, and ensure that Tor is allowed to connect to the internet. If the problem persists, execute this command `pkill -f tor` to kill the running Tor session.

**additional**
> additional:
- The **windows.py** file has been added to work on Windows

**Command to kill all running Tor sessions:**

```
pkill -9 tor
```

**Explanation of the command:**

* **pkill:** A tool for killing processes.
* **-9:** A strong kill signal sent to all running Tor processes.
* **tor:** The name of the process you want to kill.

**Notes:**

* This command will kill all running Tor sessions, including those running in the background.
* This command may not work on some operating systems.

**Alternatives:**

* You can use the task manager to kill Tor sessions manually.
* You can use a tool like ```ps aux | grep tor``` to list all running Tor processes and then use  ```kill```  or  ```killall``` to kill them.

**Tips:**

* If you are having problems with Tor, try restarting it using the command```service tor restart```.
* You can also use the command  ```tor --version```  to check the version of Tor you are using.
* If you need further assistance, you can visit the [Tor](https://www.torproject.org/)





## Contributors


- [My Facebook](https://www.facebook.com/mohmed.nabil.90813)
## Screenshot

![Screenshot_٢٠٢٤٠٣٠٥-١٥٢٦٣٧_Termux](https://github.com/Mohamed9x60/TorVpn/assets/162137526/0c75391c-016b-4bee-b946-f9a9d713b473)




## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

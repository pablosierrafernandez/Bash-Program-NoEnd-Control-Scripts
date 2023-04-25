# Bash-Program-NoEnd-Control-Scripts
🛑This repository contains three Bash scripts to control a process called `senseFi`. The scripts are used to stop and start `senseFi` processes and manage their PIDs.
# Bash Program: SenseFi Control Scripts

This repository contains three Bash scripts to control a process called `senseFi`. The scripts are used to stop and start `senseFi` processes and manage their PIDs. The scripts are:

1.  `atura_senseFi.sh`: Stops `senseFi` processes and stores their PIDs in a text file for later use.
    
2.  `activa_seseFi.sh`: Starts previously stopped `senseFi` processes by reading the PID numbers stored in the text file created by `atura_senseFi.sh`.
    
3.  `senseFi.sh`: A simple script to execute the `senseFi` process.
    

## Usage

### Stop `senseFi` Processes

To stop all `senseFi` processes, run `atura_senseFi.sh` with no arguments.

`./atura_senseFi.sh` 

### Start `senseFi` Processes

To start previously stopped `senseFi` processes, run `activa_seseFi.sh` with no arguments.

`./activa_seseFi.sh` 

### Execute `senseFi`

To execute the `senseFi` process, simply run `senseFi.sh`.

`./senseFi.sh` 

## Notes

-   These scripts were created and tested on a Linux-based operating system.
    
-   The `atura_senseFi.sh` script uses the `sudo` command to kill `senseFi` processes, so you may need to enter your password when running the script.
    
-   The `activa_seseFi.sh` script also uses the `sudo` command to start `senseFi` processes.
    
-   The PIDs of stopped `senseFi` processes are stored in a text file called `PID_Parados.txt` in the `/home/milax/` directory. If this file does not exist when `activa_seseFi.sh` is run, no processes will be started.
    
-   The `senseFi.sh` script simply executes the `senseFi` process and prints its PID to the console.
    
-   These scripts are provided as-is, without any warranty or guarantee of functionality. Use them at your own risk.

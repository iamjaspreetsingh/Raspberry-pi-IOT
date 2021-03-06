# Raspberry-pi-IOT
The complete package of Raspberry pi 
### Important Linux Commands
#### man  [command] 
Shows the Manual for the particular command and its options
#### pwd 
Shows the path of the current directory
#### ls [option(s)] [file(s)]
If you run ls without any additional parameters, the program will list the contents of the current directory in short form.
-l        detailed list
-a        displays hidden files


#### cp [option(s)] sourcefile targetfile
Copies sourcefile to targetfile.
-i     Waits for confirmation, if necessary, before an existing targetfile is overwritten
-r      Copies recursively (includes subdirectories)

#### mv [option(s)] sourcefile targetfile
Copies sourcefile to targetfile then deletes the original sourcefile.
-b  Creates a backup copy of the sourcefile before moving
-i   Waits for confirmation, if necessary, before an existing targetfile is overwritten

#### rm [option(s)] file(s)
Removes the specified files from the file system. Directories are not removed by rm unless the option -r is used.
-r  Deletes any existing subdirectories
-i  Waits for confirmation before deleting each file.

#### cd [options(s)] [directory]
Changes the current directory. cd without any parameters changes to the user's home directory.
#### mkdir [option(s)] directoryname
Creates a new directory.
#### rmdir [option(s)] directoryname
Deletes the specified directory, provided it is already empty.
#### locate pattern(s)
The locate command can find in which directory a specified file is located. If desired, use wild cards to specify file names. The program is very speedy, as it uses a database specifically created for the purpose (rather than searching through the entire file system). This very fact, however, also results in a major drawback: locate is unable to find any files created after the latest update of its database.
The database can be generated by root with updatedb.
#### updatedb [options(s)]
This command performs an update of the database used by locate. To include files in all existing directories, run the program as root. It also makes sense to place it in the background by appending an ampersand (&), so you can immediately continue working on the same command line (updatedb &).
#### cat [option(s)] file(s)
The cat command displays the contents of a file, printing the entire contents to the screen without interruption.
-n  Numbers the output on the left margin

#### date [option(s)]
This simple program displays the current system time. If run as root, it can also be used to change the system time. Details about the program are avail
#### ping [option(s)] host name|IP address
The ping command is the standard tool for testing the basic functionality of TCP/IP networks. It sends a small data packet to the destination host, requesting an immediate reply. If this works, ping displays a message to that effect, which indicates that the network link is basically functioning.

#### ip a
The ip command prints all the details of the network adapters including the IP, gateway and MAC Address
passwd [option(s)] [username]

Users may change their own passwords at any time using this command. Furthermore, the administrator root can use the command to change the password of any user on the system.
#### poweroff 
#### Shut Down command 
#### reboot [option(s)]
restarts the system
#### clear
This command cleans up the visible area of the console. It has no options.
#### reset
This command cleans up the entire console. It has no options. <br>

## Creating an SSH connection with the Raspberry Pi
	Install TeraTerm 
	Click File  --> New connection, 
	Select TCI/IP Connection
	Then type in your Raspberry Pi’s IP 

\
	Click OK with the default settings
	Click Continue for the Security Key Question
	Enter the Username as pi
	Enter the Password as password
	Click OK to login in to the Raspberry Pi SHELL
Creating a VNC connection with the Raspberry Pi
	
  Install TightVNC viewer in your system
	Open your TightVNC Viewer 
	Type in the IP of your raspberry Pi  followed by the Display Number
	The default display Number is 1
	Click Connect with the Default settings
	When asked for password enter the default password “password”
	It would open a VNC connection with the raspberry Pi
	The Raspberry Pi is installed with Raspbian OS and the default desktop environment is PIXEL
## Hardware Components and Details

Raspberry Pi’s GPIO Details , 8 BIT CHAR LCD PIN Details  ,HC-SR04  ULTRASONIC SENSOR PinOut  Details , DHT11 PINOUT ,  IR SENSOR PINOUT DETAILandRELAY MODULE PINOUT DETAILS
 is given in provided images 


## PROJECT EXECUTIONS

All the scripts for the all Projects for the workshop are stored in the /home/pi/Projects folder

It is advised to run those scripts in SHELL or in a terminal or via SSH

It is advised to run those scripts as a super user because some of the projects require admin permission to execute certain system processes

Enter the Projects Directory  using the following command

	cd /home/pi/Projects

Please verify that your current directory is /home/pi/Projects by using the following command. This command will print the current directory path

pwd

Use the following command to run any project script file
	sudo python script_filename

Press CTRL + C to interrupt the execution

Project Execution in the PIXEL Desktop Environment

If you feel comfortable in using the desktop environment than the shell environment please follow the steps to run them

Open the /home/pi/Projects folder in the UI

Double Click on the python script file. By default it opens in the PYTHON 2.x editor

If the system opens the file in a different editor then right click -> Open with PYTHON 2.x editor

Once opened press F5 key to run the Python Script

Not all the programs would execute because certain scripts need sudo permissions

## PRECAUTION
Whenever you want to connect the Project circuit Please Poweroff the Raspberry Pi using the following command and wait till only the red LED glows constantly
sudo poweroff
#### For further details , Open the Manual.doc provided

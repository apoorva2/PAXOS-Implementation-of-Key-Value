# PAXOS-Implementation-of-Key-Value

---------------------------------------------------------------------------------------------------------------------------
Important Notes
----------------------------------------------------------------------------------------------------------------------------
1) The makefile submitted here, uses "mcs" to compile the C sharp code. This compiler is specific to Mono tool and consequently we need to install the mono tool. It can be downloaded from : http://www.mono-project.com/.

2) The bin folder (the executables containing folder) needs to be added to "PATH" environment variable.
This is required to run C# compiler "mcs". For windows the bin folder path is "C:\Program Files (x86)\Mono\bin"

THE STEPS #1 AND #2 ARE OPTIONAL AND CAN BE SKIPPED IF THE MONO IS ALREADY INSTALLED.

3) Cygwin terminal is required to be used for executing the makefile in a Windows machine.
STEP #3 IS NOT RELEVANT FOR LINUX MACHINE

4) Execute the makefile provided in the bundle to compile the code for each node. The bundle includes both the server and the client application.

5) During the execution of the process, below are the files that are created. Please note that each of this file is created in the same folder location as the executable(the executable shall be created in the same location as the project folder).
	a) KeyValue file - To store the key and the values entered using the PUT process.
	b) Log File - To store the server loggings.
	c) ClientLog File - To store the client loggings.
--------------------------------------------------------------------------------------------------------------------------------------------------
Components
--------------------------------------------------------------------------------------------------------------------------------------------------
1. Client: This is the Source Code for Client Application.
2. RemoteServer: Solution Folder has two projects: TCP Server Application and UDP Server Application
3. TwoPhaseServer: This class library is called remotely from the client via HTTP and it internally uses "RemoteMethods" to do the core operations. This library also has the definition to communicate to other peer servers.
4. RemoteMethods: Class library that has definition of the three core operations(GET, PUT, Delete).
4. Makefile
5. Executive Summary

--------------------------------------------------------------------------------------------------------------------------------------------------
How to run
--------------------------------------------------------------------------------------------------------------------------------------------------
1. ADD the Server names (along with port numbers) in the APP.CONFIG on the "RemoteServer" and "Client". 

2. The first server IP and PORT NUMBER should be of the leader

3.  Server: Run the executable from the command prompt by passing the port number as the parameter. The port number should be same as the one in App.config files.

4. Client: Run the executable from the command prompt (Client.exe). 
   Client is an interactive console application.
    

 

# SelfMon VirtualKeypad
SelfMon Java Based VirtualKeypad - For local network use with all Galaxy panels configured with an Ethernet module.

You may download this software for personal non-commercial use, but you must not distribute without prior agreement from SelfMon Ltd. There is a
fully secured end to end version of this software written in 'C', which runs on the SelfMon Ltd platform and is available under commercial license.

You will need to install a Java Runtime Environment on your operating system of choice.

Running the program:

java -jar VirtualKeypad.jar -paneladdr=<IP/hostname> -httpport=<port> -panelport=<port> -timing=<read delay> -auth=<user:pass> -timeout=<seconds>

Example: 
java -jar VirtualKeypad.jar -paneladdr=10.0.0.20 -httpport=82 -panelport=10006  -timing=600 -auth=daddy:loveswhisky

The following command parameters are optional and have the following defaults:
-paneladdr=10.226.111.19 (replacing 10.226.111.19 with your panel IP address or resolvable name)
-httpport=80 (standard browser http port)
-panelport=10001 (the default port on the Galaxy)
-timing=150 (150 milliseconds delay between write and read. Good for a local LAN)
-timeout=150 (150 second virtual keypad incativity period disconnect from panel. 0 = no timeout)
-rsscode=password (The communications->password set in RSS to connect to the panel. Default is no password set)
-auth=  (when -auth is not specified, there is NO web page AUTHENTICATION required at the web browser)

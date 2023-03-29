Port Scanner

This is a simple Python script that scans a target IP address for open ports. It takes in a target IP address and a number of ports to scan, and then iterates over each port to check if it is open or closed.

The script uses the socket module to create a socket and attempt to connect to each port using the sock.connect() method. If the connection is successful, it prints a message indicating that the port is open. If the connection is not successful, it simply passes over the port and continues scanning.

The script also includes a timeout of 0.5 seconds for each connection attempt, using the sock.settimeout() method. This ensures that the script does not get stuck waiting for connections that take too long to establish.

To run the script, simply clone the repository and run python port_scanner.py in your terminal. You will be prompted to enter a target IP address and a number of ports to scan.

This script can be used for basic network reconnaissance and vulnerability assessment, and can help identify potential entry points for attackers. However, it should be used with caution and only on networks that you have permission to scan.

Screenshot:
![image](https://user-images.githubusercontent.com/108234550/228676639-95a69d49-cfdd-4ce2-b991-60bb6dfefe87.png)

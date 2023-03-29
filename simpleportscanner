import socket
import termcolor


def scan(target, ports):
    print('\n' + ' Starting Scan for ' + str(target))
    for port in range(1, ports):
        scan_port(target, port)


def scan_port(ipaddress, port):
    try:
        sock = socket.socket()
        sock.settimeout(0.5)  # Add a timeout of 0.5 seconds
        sock.connect((ipaddress, port))
        print("[+] Port Opened" + str(port))
        sock.close()
    except:
        pass


targets = input("[*] Enter the targets (Split them by ,): ")
ports = int(input("[*] How many ports do you want to scan? "))
if ',' in targets:
    print(termcolor.colored("[*] Scanning Multiple targets", 'green'))
    for ipa in targets.split(','):
        scan(ipa.strip(), ports)
else:
    scan(targets, ports)

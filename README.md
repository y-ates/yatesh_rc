| Command                | Description                                                                                                      | Usage Example                                 |
|------------------------|------------------------------------------------------------------------------------------------------------------|-----------------------------------------------|
| **ll**                 | Lists files in the current directory with additional information (detailed, human-readable format).             | `ll`                                          |
| **c**                  | Copies command output directly to the clipboard using `xclip`.                                                  | `echo "Hello" | c`                            |
| **server**             | Starts an HTTP server on the specified port and directory (defaults to the current directory if not specified).  | `server 8080 ./mydir`                         |
| **rs**                 | Generates a reverse shell script.                                                                               | `rs 192.168.1.10 4444 > shell.sh`            |
| **con_htb**            | Connects to Hack The Box VPN using a specific `.ovpn` file.                                                     | `con_htb`                                     |
| **htb-init**           | Initializes Hack The Box (HTB) directory structure and starts an HTTP server in the `share` folder.             | `htb-init <machine_name>`                    |
| **nmap-full**          | Runs a comprehensive `nmap` scan on all ports with common scripts and service/version detection.                | `nmap-full 10.10.11.169`                     |
| **addhost**            | Adds an IP and domain to `/etc/hosts`, appending to an existing entry if necessary.                             | `addhost 192.168.1.10 example.local`         |
| **nmap_udp**           | Runs an `nmap` UDP-only scan, saving output in the `nmap` directory with specified options.                     | `nmap_udp 10.10.11.169`                      |
| **ffuf-dir**           | Runs a directory brute-force scan using `ffuf` with a large wordlist.                                           | `ffuf-dir http://site.com/FUZZ`              |
| **ffuf-vhost**         | Performs a virtual host discovery scan using `ffuf` with a subdomain wordlist.                                  | `ffuf-vhost example.com`                     |
| **st**                 | Stabilizes a reverse shell session by spawning a `pty` and setting `TERM`. Output is copied to clipboard.       | `st 1`                                       |
| **mcd**                | Creates a new directory and immediately changes into it.                                                        | `mcd new_folder`                             |

# quick-socks-proxy

Running a SOCKS proxy locally can be done using various tools and software. One of the simplest and most commonly used methods is to use ssh (Secure Shell) to create a SOCKS proxy. Here’s a step-by-step guide to running a SOCKS proxy locally using ssh:

Using ssh
Requirements:
ssh client installed (available by default on most Unix-like systems, including Linux and macOS. For Windows, you can use OpenSSH or tools like PuTTY).
Steps:
Open a Terminal (Command Prompt or PowerShell on Windows, Terminal on macOS or Linux).

Run the ssh command to create the SOCKS proxy. Use the following syntax:

sh
Copy code
```
$ ssh -D [local_port] [user]@[remote_host]
```
-D [local_port]: This option specifies the local port on which the SOCKS proxy will listen. For example, -D 1080 will make the proxy listen on port 1080.
[user]: Your username on the remote machine.
[remote_host]: The address of the remote machine you are connecting to.
Example:

sh
Copy code
```
ssh -D 1080 user@example.com
```
This command will create a SOCKS proxy on localhost:1080. You will need to authenticate with your SSH credentials.

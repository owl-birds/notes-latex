https://www.youtube.com/watch?v=hQWRp-FdTpc 

# SSH (Secure Shell)

- Secure Shell 
- Communication Protocol (like http/s, ftp, etc)
- do anything that u want remotely, but its encrypted
- traffic is encrypted
- used mostly in the terminal/command line 

## ->
- SSH is the client 
- SSHD is the server (open SSH Daemon)
- the server must have sshd installed and running or you wil not be able to
connect using SSH 

### Authentication method

:::> ssh user@local-ip-address 

- password
- Public/Private Key pair 
- Host Based 

# Generating Keys

:::> ssh-keygen

- ~/.ssh/id_rsa (Private Key)
- ~/.ssh/id_rsa.pub (Public Key)
- Public Key goes into server textbf{"autherized_keys"} file

# what about windows

- windows start support native SSH on windows 10 
- putty was used in older versions of windows 
- git bash & other terminal programs include the ssh commmand & other Unix
tools



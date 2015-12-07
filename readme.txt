-----------------------------sshkeygen v1.0--------------------------
Function introduction:
This shell script is used to bulid trust relationship between linux hosts.After the scripts executed ,you can execute "scp" or "ssh" command without input password.

Usage:
1.Upload all script file to the Linux host.

2.Edit the "iplist.txt" file format as follows

192.168.20.191;root;fnst1234
192.168.20.192;root;fnst1234
192.168.20.193;root;fnst1234
192.168.20.194;root;fnst1234

3.bulid the trust relationship 

(1) single trust relationshio between Linux hosts
    sh create-keygen-remote.sh -i iplist.txt

(2) Mutual trust relationship between Linux hosts
    sh create-keygen.sh -i iplist.txt

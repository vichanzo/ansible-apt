This is my version of Locally run Ansible for apt based installs.

First install the basics:
```bash
sudo apt update
sudo apt install open-sshserver git ansible
```

Create / import your private key:
```bash
nano ~/.ssh/id_rsa
```
Create /import your public key:
```bash
nano ~/.ssh/id_rsa.pub
```

Test your keys with git:
```bash
ssh -T git@github.com
```

Clone this repository:
```bash
git clone git@github.com:vichanzo/ansible-apt.git
```

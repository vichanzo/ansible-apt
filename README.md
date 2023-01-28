### Readme

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

Create a file with "nano test-commit.txt" then push it to git.
```
git status
git add test-commit.txt
git commit -m "first commit"
git push origin main
```


Run the ansible playbook
```
ansible-playbook local.yml
```


#### Reference: 
- https://thesmarthomejourney.com/2021/09/06/home-server-basics-ansible/
- [github rbq/docker.yaml](https://gist.github.com/rbq/886587980894e98b23d0eee2a1d84933)
- [perfectmediaserver.com](https://perfectmediaserver.com/installation/manual-install-ubuntu/)



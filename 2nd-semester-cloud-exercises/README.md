# Exercise on Users and Group Management Task on Linux

## Task Overview

- Create three groups: `admin`, `support`, and `engineering`.
- Add the `admin` group to the sudoers file.
- Create a user in each group.
- Generate SSH key for the `admin` user.
- Submit the relevant system file contents.

---

## Get vagrant running and run the Linux commands for Groups/users to be Created

```bash
sudo groupadd admin
sudo groupadd support
sudo groupadd engineering

sudo useradd -m -G admin adminuser
sudo useradd -m -G support supportuser
sudo useradd -m -G engineering enguser

---

## Generated key is located in /home/adminuser/.ssh/id_rsa and /home/adminuser/.ssh/id_rsa.pub

sudo su - adminuser
ssh-keygen

---
## Sudoers configuration

%admin ALL=(ALL:ALL) ALL


--

## File snippt

$(cat passwd_snippet.txt)

---

## Submitted by Adada Edia

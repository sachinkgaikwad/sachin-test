# sachin-test

Requirements :
aws account 

micro ec2 instance --2 .

Ansbile installed on manage / control machine . 

---
#steps 
---

1.Git clone https://github.com/sachinkgaikwad/sachintest/

2.Make sure you have passwordless connumnication beetwen both machine. 

3.Add /etc/hosts entry for machine to manage . 

4.Rpdate inventor/hosts for new user to manage .

5.Run following command to add new user and grant ssh access  : ansible-playbook -i inventory/ -e "action=grant" playbooks/ssh.yml

6.Run to remove user and ssh access : ansible-playbook -i inventory/ -e "action=revoke" playbooks/ssh.yml

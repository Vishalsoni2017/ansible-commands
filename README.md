1. ansible devservers -i /root/hosts -a "ls -l"  -> -i for inventory file <br>
2.  ansible localhost -i hosts -m ping  --> -m for ping module <br>
3. ansible-inventory -i /root/hosts --list
4. ansible-inventory -i /root/hosts --graph
5. ansible-inventory -i /root/hosts --list -y
6. ansible servers -i hosts -m setup -a "filter=ansible_distribution"
7. ansible servers -i hosts -m setup -a "filter=ansible_date_time"
8. ansible servers -i hosts -m file -a "path=/opt/deployment state=directory"
9. ansible servers -i /root/hosts -m copy -a 'src=/root/configfile.cfg dest=/opt/deployment'
10. ansible servers -i /root/hosts -m lineinfile -a "path=/opt/deployment/configfile.cfg regexp='^var1' line='var1=111111'"
11. ansible servers -i /root/hosts -m shell -a 'cat /opt/deployment/configfile.cfg'
12. ansible servers -i hosts -m shell -a "sed -i 's/var1=000000/var1=111111/g' /opt/deployment/configfile.cfg"

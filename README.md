1. ansible devservers -i /root/hosts -a "ls -l"  -> -i for inventory file <br>
2.  ansible localhost -i hosts -m ping  --> -m for ping module <br>
3. ansible-inventory -i /root/hosts --list
4. ansible-inventory -i /root/hosts --graph
5. ansible-inventory -i /root/hosts --list -y

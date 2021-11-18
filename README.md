# bash-tips

id.id.ip 10.101.10.10


IFS=$'\n'; for lin1 in $(cat posleden_vals); do min_id=$(echo "$lin1"| cut -d " " -f1); ip1=$(echo "$lin1"| cut -d " " -f2);  ssh -o StrictHostKeyChecking=no -i ~/.ssh/id_rsa_maas2 maas@$ip1 "sudo sed -i 's/^id\:.*/id\: $min_id/g' /etc/salt/etc/minion" ; do




Mkpart script

Script creates a partition on  the whole disk, format it in ext4, make mount point , mount disk and adds a row for it in etc fstab


Audit_serv

Run commands on list of servers and collets output in files



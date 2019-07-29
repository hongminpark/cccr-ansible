```
[vagrant@controller ~]$ history
    1  ll
    2  pwd
    3  whoami
    4  cat /etc/passwd
    5  TMOUT=0
    6  ls -alrt
    7  whoami
    8  cat /etc/*release*
    9  sudo --help
   10  su
   11  sudo -i
   12  ll
   13  exit
   14  sudo -i
   15  ansible all -m ping
   16  ssh-keygen
   17  ls .ssh/
   18  ssh-copy-id  vagrant@host1
   19  ssh-copy-id vagrant@host1
   20  ssh-copy-id vagrant@host2
   21  ssh-copy-id vagrant@controller
   22  history
   23  ansible all -m ping
   24  ll
   25  ls
   26  ls -alrt
   27  cd .ssh/
   28  ll
   29  cat known_hosts
   30  vi known_hosts
   31  ssh host1
   32  cat known_hosts
   33  ll
   34  cat authorized_keys
   35  ll
   36  cat id_rsa
   37  cat id_rsa.pub
   38  cd
   39  ansible all -m command -a "hostname"
   40  ansible all -m command -a "id"
   41  ansible all -m command -a "whoami"
   42  ansible all -m command -a "cat /etc/passwd"
   43  ansible all -m command -a "cat /etc/passwd" | grep root
   44  ansible all --list-hosts
   45  ansible ungrouped --list-hosts
   46  ansible host* --list-hosts
   47  cd /etc/host
   48  cd /etc/ansible/
   49  ll
   50  pwd
   51  mkdir host_vars
   52  sudo mkdir host_vars group_vars
   53  ll
   54  cd host_vars/
   55  touch foosball
   56  sudo touch foosball
   57  ll
   58  cd ../
   59  ll
   60  cd group_vars/
   61  ll
   62  touch raleigh
   63  sudo tough raleigh webservers
   64  sudo touch raleigh webservers
   65  ll
   66  ansible all --list-hosts
   67  sudo vi /etc/ansible/hosts
   68  ansible all --list-hosts
   69  ansible ungroupd --list-hosts
   70  ansible raleigh --list-hosts
   71  ansible southeast --list-hosts
   72  ansible atlanta:raleigh --list-hosts
   73  ansible atlanta.raleigh --listhosts
   74  ansible atlanta.raleigh --list-hosts
   75  ansible host1.host2.host3 --list-hosts
   76  ansible host1,host2,host3 --list-hosts
   77  ansible atlanta:&raleigh --lsit-hosts
   78  ansible 'atlanta:&raleigh' --lsit-hosts
   79  ansible 'atlanta:&raleigh' --list-hosts
   80  ansible atlan* --list-hosts
   81  which ansible
   82  cd /usr/bin/
   83  ll | grep ansible
   84  cd /usr/bin/
   85  vi ansible-2.7
   86  cd /etc/ansible/
   87  ll
   88  ansible --help
   89  ansible -i
   90  ll
   91  cd group_vars/
   92  ll
   93  touch southeast
   94  sudo touch southeast atlanta
   95  sudo rm webservers
   96  ll
   97  cd ../
   98  ll
   99  cd host_vars/
  100  ll
  101  sudo rm foosball
  102  sudo touch host1 host2
  103  ansible inventory --list
  104  ansible-inventory --list
  105  ansible-inventory --graph
  106  ansible-inventory --host host1
  107  ansible-inventory --host host2
  108  ansible-inventory --group southeast
  109  ansible-inventory --groups southeast
  110  ansible-inventory --help
  111  ansible-inventory --list --yaml
  112  ll
  113  cd ../
  114  ll
  115  cd group_vars/
  116  ll
  117  vi atlanta
  118  sudo vi atlanta
  119  sudo vi raleigh
  120  sudo vi southeast
  121  ansible-inventory --list
  122  sudo vi atlanta
  123  sudo vi raleigh
  124  sudo vi southeast
  125  ansible-inventory --list
  126  ansible-inventory --host host1
  127  ansible-inventory --host host2
  128  ansible-inventory --host host3
  129  sudo rm atlanta
  130  ll
  131  sudo mkdir atlanta
  132  sudo vi var1.yaml
  133  cat "var2: abc" > var2yaml
  134  sudo cat "var2: abc" > var2yaml
  135  sudo cat "var2: abc" > var2.yaml
  136  ll
  137  sudo mv var1.yaml atlanta/
  138  cd atlanta/
  139  ll
  140  sudo vi var2.yaml
  141  ansible-inventory --hosts host1
  142  ansible-inventory --host host1
  143  ansible-doc -t connection -l
  144  ansible-doc --help
  145  ansible-doc -l
  146  ansible-doc -l | wc -l
  147  cd /usr/lib/python2.7/
  148  cd site-packages/
  149  cd ansible
  150  ll
  151  cd module
  152  ll
  153  cd modules/
  154  ll
  155  cd system/
  156  ll
  157  cd ./
  158  ll
  159  cd ./
  160  cd ../
  161  ll
  162  ansible-doc copy
  163  cd /etc/ansible/
  164  ll
  165  sudo rm -rf hosts group_vars/ host_vars/
  166  ll
  167  sudo vi hosts
  168  ansible host1 -a 'hostname'
  169  ansible host1 -a 'hostname' -u root
  170  ansible host1 -a 'hostname' -u root -b
  171  ansible host1 -a 'hostname' -u vagrant
  172  ansible host1 -a 'hostname' -u vagrant --ask-pass
  173  ansible host1 -a 'hostname' -u root --become-user
  174  ansible host1 -a 'hostname' --become-user root
  175  ansible --help
  176  ansible host1 -a 'id' -b
  177  ansible host1 -a 'id'
  178  cd
  179  echo "Hello world" > hello.txt
  180  ansible host1 -m copy -a "src=hello.txt dest=/tmp/"
  181  vi hello.txt
  182  ansible host1 -m copy -a "src=hello.txt dest=/tmp/"
  183  ansible host1 -m copy -a "content='Helloooo' dest=/tmp/hello.txt"
  184  ansible host1 -a "cat /tmp/hello.txt"
  185  ansible atlanta --list-hosts
  186  ansible host1 -m copy -a "src=/etc/hosts dest=/tmp/hosts"
  187  ll /etc/hosts
  188  ansible host1 -m file -a "dest=/tmp/hosts mode=600"
  189  ansible host1 -m file -a "dest=/tmp/hosts mode=600 owner=root"
  190  ansible host1 -m file -a "dest=/tmp/hosts mode=600 owner=root" -b
  191  ansible host1 -m file -a "dest=/tmp/hosts mode=600 state=absent"
  192  ansible host1 -m file -a "dest=/tmp/hosts mode=600 state=absent" -b
  193  ansible-doc file
  194  history
  195  cd
  196  ls -alrt
  197  vi .bash_history
  198  uptime
  199  date
  200  ansible --help
  201  ansible host1 -a "yum list httpd"
  202  ansible host1 -m yum -a "name=httpd state=installed" -b
  203  cat /etc/shadow
  204  sudo cat /etc/shadow
  205  sudo cat /etc/shadow | grep vagrant
  206  sudo grep vagrant /etc/shadow
  207  ansible host1 -m service -a "name=httpd state=started" -b
  208  ansible host1 -a "systemctl status httpd"
  209  systemctl status httpd
  210  ansible host1 -m service -a "name=httpd state=restarted" -b
  211  ansible host1 -a "systemctl status httpd"
  212  ansible all -m setup
  213  ansible all -m setup | grep partition
  214  history
  ```

#### ansible-plabook options
    -K: sudo password on target server
    -k: user password
    -f: default num = 5
    -i: hosts files. default path = /etc/ansible/

#### edit ./hosts whrn localhost is target
    [addnew]
    127.0.0.1
    x.x.x.x

#### edit ./hosts whrn localhost is not targets
    [addnew]
    x.x.x.x
    y.y.y.y

#### edit ./centos7.yml
    - hosts: addnew

#### setup target server
    $ ansible-playbook  -i ./hosts -K ./centos7.xml



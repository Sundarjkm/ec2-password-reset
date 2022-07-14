# ec2-password-reset

create iam role
aws service > use case as ec2>attach a AmazonSSMManagedInstanceCore policy>
give a role name>create

Attach IAM role for ec2 instance
select instance then actions -> security ->modify IAM role>select the role u previosely created 

choose the ec2 instance then connect choose session manager then connect

you can get your instance powershell access


enter
cmd
if you want reset the administrator user password follow this

syntax
net user USERNAME *
type the password twice

example 
net user administrator *


if you want create the user add to groups follow this steps
syntax
net user /add [*username] [password]
net localgroup administrators [username] /add
net localgroup "remote desktop users" [username] /add


exampleuser
net 
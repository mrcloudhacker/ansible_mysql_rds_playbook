# ansible_mysql_rds_playbook

This is a playbook which can be used as an example to create mysql master,read replica and upgrade the read replica on RDS.

### Remember..!!
* Running for the first time exclude the task 'upgrade' as it will immediately upgrade the read replica to the mentioned version,
  you can do so by executing
  `ansible-playbook -vvv rds.yml --skip-tags "upgrade"`
  
* This playbook has authentication information encrypted, so use this command while firing this playbook 
   `ansible-playbook -vvv rds.yml --ask-vault-pass`
   Use the pass `codin` to get the access :P


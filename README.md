Rename following files by removing _sample

  aws_keys_sample.yml
  vars_sample.yml
  setup_sample.json


As a best practice, aws_keys.yml should be encrypted using vault for instance: 
```
ansible-vault encrypt aws_keys.yml
```


To run the playbook:
```
ansible-playbook aws_avicontroller.yml --ask-vault
```

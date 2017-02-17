To demonstrate the issue in https://github.com/ansible/ansible/issues/21513

```
time ansible-playbook recursive.yml -i localhost, -c local                                              
rm -rf dest/*
time ansible-playbook with_items.yml -i localhost, -c local
```

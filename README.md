# Ansible Role: django

Deploy python django apps inside a docker container. There are 2 docker container created by this ansible roles, which is nginx and another box for running the python uwsgi module

## Requirements

CentOS 7 Minimal Installation with docker installed

## Example Playbook

`django.yml`

    - hosts: all
      remote_user: root
      roles:
        - django

Running playbook on specific hosts:

    ansible-playbook -i host1.example.com,host2.example.com django.yml

## License

MIT

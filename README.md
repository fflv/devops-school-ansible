# Задания по Ansible

Подкорректирован исходный Vagrantfile, добавлена установка на control-node git и ansible
В остальных аспектах тестовый стенд не изменялся

Каждое задание вынесено в отдельную роль и обозначено тэгом
## Задание №1

Чтобы запустить все задания последовательно

`ansible-playbook -i inventory.ini playbooks/001-task.yml` 

Чтобы запустить задание по тэгу

`ansible-playbook -i inventory.ini playbooks/001-task.yml --tags 103`

По умолчаниию в тестируемой версии CentOS присутствовали параметры в /etc/default/grub. Чтобы задание отработало - нужно убрать хотя бы один параметр вручную.


## Задание №2

`ansible-playbook -i inventory.ini playbooks/002-task.yml --ask-vault-pass` 

Пароль ansible-vault: vagrant

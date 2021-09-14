## Домашнее задание к занятию "8.4 Работа с Roles"
***

> Предварительно создал новые репозитории для ролей и playbook
***
### Задание 1-2
```
falconow@falconow:~/lesson/ansible_8.4$ ansible-galaxy install -r requirements.yml -p roles/
Starting galaxy role install process
- extracting elastic to /home/falconow/lesson/ansible_8.4/roles/elastic
- elastic (2.0.0) was installed successfully
```
***
### Задание 3
```
 falconow@falconow:~/lesson$ ansible-galaxy role init --force kibana-role/
- Role kibana-role/ was created successfully
falconow@falconow:~/lesson$ 
```
### Задание 4-12
> Создал новые роли командой выше для установки kibana и filebeat. Перенс task из playbook
> в соответствующие роли. Заполнил переменные vars, перенес шаблоны. 

> Создал файлы requirements и скачал роли в playbook
>> Команда на скачивание роли filebeat:
```
ansible-galaxy install -r requirements_filebeat.yml -p roles/ --force
Starting galaxy role install process
- changing role filebeat from main to main
- extracting filebeat to /home/falconow/lesson/ansible_8.4/roles/filebeat
- filebeat (main) was installed successfully
```

> Переписал playbook на использование ролей


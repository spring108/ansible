## DevOps \ Домашнее задание №8 - Ansible

Написать playbook, который подготавливает сборочное и продовое окружение на 2-х нодах. 
На сборочной ноде производится сборка проекта, на продовой - запуск. 


## Команды на Master:
  - #### Подготовка инфраструктуры:
    - sudo apt update
    - sudo apt-get update
    - sudo apt-get install mc -y
    - sudo mc
  - #### Запуск сервисов:
    - cd /tmp
    - git clone https://github.com/spring108/ansible.git
    - cd /tmp/ansible

## Команды на Slave1:
  - #### Подготовка инфраструктуры:
    - sudo apt install python

## Команды на Slave2:
  - #### Подготовка инфраструктуры:
    - sudo apt install python

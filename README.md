## DevOps \ Домашнее задание №8 - Ansible

Написать playbook, который подготавливает сборочное и продовое окружение на 2-х нодах (Ubuntu 18.04). На сборочной ноде производится сборка проекта, на продовой - запуск. 


## Команды на Slave1 & Slave2:
  - #### Подготовка инфраструктуры:
    - Настройка авторизации по ключам от Master
      - sudo nano /etc/ssh/sshd_config
      - sudo service sshd restart
      - sudo passwd root
    - sudo apt install python -y


## Команды на Master:
  - #### Подготовка инфраструктуры:
    - sudo apt update
    - sudo apt-get update
    - sudo apt-get install mc -y
    - sudo mc
    - Настройка авторизации по ключам до Slave1 и Slave2
      - ssh-keygen
      - ssh-copy-id /root/.ssh/id_rsa.pub root@Slave1
      - ssh-copy-id /root/.ssh/id_rsa.pub root@Slave2
    - sudo apt update
    - apt policy ansible
    - sudo apt install ansible -y
    - ansible --version #ansible 2.5.1
  - #### Запуск сервисов:
    - cd /tmp
    - git clone https://github.com/spring108/ansible.git
    - cd /tmp/ansible


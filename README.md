# Домашнее задание к занятию "9.1. «Система мониторинга Zabbix»" - Соловьёв Андрей SYS-18

При выполнении задания в качестве Zabbix-serverиспользована домашняя машина.
Zabbix-agent установлен на две виртуальные машины 

192.168.122.104 

192.168.122.198

---

## Задание 1

Установите Zabbix Server с веб-интерфейсом.

### Процесс выполнения

1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. Установите PostgreSQL. 

![PostgressSQL](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Postgresssql.png)

3. Пользуясь конфигуратором комманд с официального сайта, составьте набор команд для установки последней версии Zabbix с поддержкой PostgreSQL и Apache

![Zabbix_Ubuntu](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Zabbix-Ubuntu.png)

4. Выполните все необходимые команды для установки Zabbix Server и Zabbix Web Server

![Zabbix install 1](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Inst_zabbix1.png)

![Zabbix install 2](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Inst_zabbix2.png)

Zabbix-server запущен

![Zabbix-server](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/main_zabbix_server.png)


### Требования к результаты

- Прикрепите в файл README.md скриншот авторизации в админке

![Zabbix admin](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/admin.png)

![Zabbix admin2](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/gui_zabbix_server.png)


## Задание 2

Установите Zabbix Agent на два хоста.

Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. Установите Zabbix Agent на 2 виртмашины, одной из них может быть ваш Zabbix Server

Zabbix-agent запущен

![Zabbix-agent1](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/mint_zabbix_agent.png)

![Zabbix-agent2](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/xubuntu_zabbix_agent.png)


3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов
4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Server
5. Проверьте что в разделе Latest Data начали появляться данные с добавленных агентов

Требования к результату

- Приложите в файл README.md скриншот раздела Configuration > Hosts, где видно, что агенты подключены к серверу

![Zabbix conf](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Zabbix_configuration.png)

- Приложите в файл README.md скриншот лога zabbix agent, где видно, что он работает с сервером


- Приложите в файл README.md скриншот раздела Monitoring > Latest data для обоих хостов, где видны поступающие от агентов данные.

![Zabbix monitoring](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/monitoring.png)


![Mint](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Mint.png)


![Xubuntu](https://github.com/Andrewsolo1969/9-02-hw/blob/main/img/Xubuntu.png)



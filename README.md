# Практическая работа №3 WAZUH
## Выполнил студент группы ББМО-02-23 Rublev Vladimir Sergeevich

### 1. Разворачиваю виртуальную машину на базе ОС Ubuntu
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/1.jpeg)

### 2. Настраиваю на всех виртуальных машинах сетевой мост, чтобы они друг друга видели. 
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/2.jpeg)

### 3. Захожу на обе виртуальные машины и пингую друг друга для проверки соединения.  
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/3.jpg)

### 4. Начинаю установку сервера Wazuh на первую хост виртуальную машину.
Команда: "curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh && sudo bash ./wazuh-install.sh -a"
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/4.jpg)

### 5. Перехоим в браузер и вписываем наш ip адрес с портом который фигурировал в логах установки (по умолчанию 443). После захода на страницу вписываем наши логин и пароль. 
Пример: "https://10.0.2.15:443"
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/6.png)

### 6. Попадаем на главный экран wazuh server.
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/7.png)

### 7. Доступ второй виртуальной машине, чтобы сделать её агентом на сервере. 
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/8.png)

### 8. Получаем сформированную команду для добавления её во вторую виртуальную машину. 
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/99.png)
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/9.jpg)

### 10. Заходим в раздел агентов, чтобы посмотреть все виртуальные машины, которые получилось подключить к серверу в виде агентов.
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/10.png)

### 11. Произвел атаку с агента на сервер. 
Программы HOIC и LOIC. 
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/11.png)
![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/11%201.png)

### 14 Создание проверки целостности файлов на wazuh server:

![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/14.jpg)

### 15 Настройка выявления уязвимостей на wazuh server:

![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/15.png)

### 16 Настройка выявления скрытых процессов на wazuh agent:

![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/16.png)

### 17 Настройка выявления SQL-инъекций на wazuh server:

![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/17.png)

### 18 Настройка выявления web shell attack на wazuh agent:

![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/18.png)

### 19 Проверка отображения обнаружения атаки в истории логов на wazuh server:

![image](https://github.com/vladimirrublev/sssl3/blob/main/screenshot/19.png)

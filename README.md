Этап 1: выбор операционной системы
 У меня на компьютере стоит Windows 10 и виртуалка с убунтой 

Этап 2:  путь к установке Vagrant
 Ситуация в мире достаточно тяжелая, из-за чего просто так скачать Vagrant не удаётся. Необходимо искать пути обхода и я выбрал путь VPN. Остановился на Windscribe VPN, так как он бесплатный и прекрасно себя показывает : ![image](https://user-images.githubusercontent.com/90474388/172420458-b3fcc349-66f3-4073-b528-b48c8e51309a.png)

Теперь переходим на официальный сайт и скачиваем Vagrant без каких-либо проблем

![image](https://user-images.githubusercontent.com/90474388/172421024-e9aa275c-9f40-4273-bedb-9eb37c847753.png)
Виртуалочку

Этап 4: настройка Vagrant
Открываем папку "Мой Компьютер" и в локальном диске C: видим папочку HashiCorp. Заходим в HashiCorp/Vagrant/ И создаём папку для настройки.  Там редачим Vagrantfile и настраиваем тем самым Vagrant.  ![image](https://user-images.githubusercontent.com/90474388/172421699-0a408a75-fbb4-48ac-a278-c57226acc98e.png)

Далее создаём и редактируем скрипт provision.sh в этой же папке ![image](https://user-images.githubusercontent.com/90474388/172421994-be1f8263-115e-4b0d-a869-c5ac5da13a51.png)


Первые две строки - наш логин и пароль для Vagrant. Далее представил примерный скрипт, который выведет банальное "Hello World"

Этап 5: Работа с Vagrant
Скачиваем среду с оф. сайта Vagrant и устанавливаем. Также используем VPN.

После установки Vagrant необходимо указать среду разработки в консоли: set Path=%PATH%;"путь к exe файлу"

Для запуска машины необходимо ввести команду vagrant up

Для запуска необходим конфиг файл vagrantfile, где указаны все настройки. Его мы создали на 4 этапе

Для нормального завершения работы необходимо использовать команду vagrant halt

Для "грубого" завершения - vagrant destroy

Также можно подключать разные плагины с помощью команды vagrant plugin install "название плагина"

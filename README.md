
### 5.
> По умолчанию выделено:
> > Оперативная память 1024 МБ
> 
> > Процессоры 2

### 6.
Для добавления оперативной памяти и ресурсов процессора необходимо:
> Остановить VM: vagrant halt
 
>Отредактировать конфигурационный файл Vagrantfile: 

    config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    end
> Запустить VM:  vagrant up
 
### 8.
- за размер истории отвечает переменная. Описание данной переменной начинается на 862 строчке
- ignoreboth не записывает в файл истории команды начинающиеся с пробела и дубликат команды введеной до этого

### 9.
Описание начинается с 1091 строчки в блоке Brace Expansion

### 10.
- touch {1..100000}.txt
- Создание 300000 файлов ограничено количеством передаваемых аргументов 
> getconf ARG_MAX # Get argument limit in bytes
>> 2097152

### 11.

Проверяет что существет файл и является директорией

### 12.
```
root@vagrant:/home/vagrant# mkdir /tmp/new_path_directory/
root@vagrant:/home/vagrant# touch /tmp/new_path_directory/bash
root@vagrant:/home/vagrant# chmod +x /tmp/new_path_directory/bash
root@vagrant:/home/vagrant# export PATH=/tmp/new_path_directory:$PATH
root@vagrant:/home/vagrant# type -a bash
bash is /tmp/new_path_directory/bash
bash is /usr/bin/bash
bash is /bin/bash
```

### 13. 
at - запускает команды в определенное время

batch - запускает команды когда загрузка системы это позволяет

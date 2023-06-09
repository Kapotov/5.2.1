## Задание - 5.2. Применение принципов IaaC в работе с виртуальными машинами.

> 1. Опишите своими словами основные преимущества применения на практике IaaC паттернов.
Какой из принципов IaaC является основополагающим?

Ответ: 
IaaC - качественно новый подход к ведению дел в Ops. Это одномоментно и техническая реализация поставленной задачи, и документирование действий, настроек. Кодинг для описания инфраструктуры приводит нас к тому, что не плохо было бы разбираться в программировании, и с точки зрения получения финального продукта - программы (в рамках Ops - код инфраструктуры), и сточки зрения - а как писать код, как его структурировать, как применять эффективные методы описания логики. В данном случае работает правило: не изобретай велосипед, все что тебе нужно, уже было сделано до тебя, тебе остается знать опыт разработки IaaC, понимать когда и что использовать и осознанно, с ответственностью, применять то или иное в работе, да, всегда, остается место для творчества и реализации, но применение паттернов IaaC опоравдано оптимизационно и функционально. Вообще, основополагающем принципом, в рамках IaaC, является обеспеченеи идемпотентности. По моему мнению, именно паттерны, которые формировались в рамка развития той или технологии - квинтэссенция максимально эффективного опыта ИТ специалистов и обеспечивает стабильность получения предсказуемого постоянного результата.    

> 2. Чем Ansible выгодно отличается от других систем управление конфигурациями?
Какой, на ваш взгляд, метод работы систем конфигурации более надёжный push или pull?

Ответ: 
Ansible написан на Python, использует метод push, что не требует установки ни демонов, ни агентов, в случае с pull методом такие агенты нужны, что потенциально может быть еще одной точкой сбоя. Использует SSH без необходимости дополнительно докручивать PKI. По совокупности, все это делает Ansible простым и эффективным. 

> 3. Установить на личный компьютер: VirtualBox, Vagrant, Ansible.
Приложить вывод команд установленных версий каждой из программ, оформленный в markdown.

Ответ:

![Снимок](https://github.com/Kapotov/5.2.1/assets/123774335/30b7e6c5-5cce-4faa-bc6b-f6101588f5f5)

![Снимок1](https://github.com/Kapotov/5.2.1/assets/123774335/a20996a6-5c66-4e72-b902-744fe724b17f)



> 4. Воспроизвести практическую часть лекции самостоятельно. Создать виртуальную машину.
Зайти внутрь ВМ, убедиться, что Docker установлен с помощью команды `docker ps`

Ответ:
```
$ vagrant ssh
Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 5.4.0-91-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

 System information disabled due to load higher than 1.0


This system is built by the Bento project by Chef Software
More information can be found at https://github.com/chef/bento
Last login: Thu Jan 20 08:02:10 2022 from 10.0.2.2
vagrant@server1:~$ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```

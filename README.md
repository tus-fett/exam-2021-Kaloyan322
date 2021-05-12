# Задание изпит КМК

## Описание

Дадени са следните мрежови адреси 192.168.100.0/24 и следната топология

![Топология](https://github.com/tus-fett/exam-21/blob/main/VLSM_subnetting.jpg)

## Мрежови изсквания
1. Използвайте мрежата ```192.168.100.0/24```
1. ```LAN 11``` - 21 хоста, включително (```R1, SW11 и R11```)
1. ```LAN 12``` - 14 хоста, включително (```R1, SW12 и R12```)
1. ```LAN 32``` - 32 хоста, включително (```R2, SW21 и R21```)
1. ```LAN 22``` - 19 хоста, включително (```R2, SW22 и R22```)
2. ```WAN link``` - 2 хоста, (R1 и R2)


## Изисквания

1. Разгледайте мрежовите изисквания. 
2. Проектирайте VLSM адресна схема.
3. Подмрежите трябва да бъдат последователни и не трябва да има загуба на адреси.
4. Задайте IP адресина на хостовете и симулирайте свързаността ([GNS 3](https://www.gns3.com/) или [Cisco PT](https://www.netacad.com/courses/packet-tracer))
5. Задайте първите използваеми IP адреси в съответните подмрежи на рутера ```R1``` за двете LAN връзки и WAN връзката.
6. Задайте първите използваеми IP адреси в съответните подмрежи на ```R2``` за двете LAN връзки. Задайте последния използваем IP адрес за WAN връзката.
7. Задайте вторите използваеми IP адреси в подходящите подмрежи на комутаторите.
8. Задайте интерфейс управление на комутаторите, под формата на IP адрес. Той трябва да бъде достъпен от всички хостове.
9. Задайте на хостовете последните използваеми IP адреси в подходящите подмрежи.
10. Документирайте Вашия отговор в приложените таблици
11. Оценка - виж приложените таблици 

|                         	| Точки 	|
|-------------------------	|------:	|
| Проектиране на подмрежи 	| 10    	|
| Пълно адресиране        	| 30    	|
| Симулация               	| 20    	|
| Общо                    	| 60    	|

| Оценка         	|   Точки 	|
|----------------	|--------:	|
| Слаб (2)       	| 0 - 22  	|
| Среден (3)     	| 23 - 33 	|
| Добър (4)      	| 34 - 43 	|
| Мн. Добър (5)  	| 44 - 52 	|
| Отличен (6)    	| 53 - 60 	|


## Отговор

Документирайте Вашите отговори в приложените таблици.

### Tаблицa подмрежи 

Използвайте CIDR запис

 ИМЕ  | Брой нужни хостове | Мрежови адрес/CIDR | Първи изпозлваем адрес/CIDR | Пoследен изпозлваем адрес/CIDR | Brodcast/ CIDR | Брой хостове
------|----------|---------|----------|------|---------|----------
LAN 11|----------|---------|----------|------|---------|----------
LAN 12|----------|---------|----------|------|---------|----------
LAN 32|----------|---------|----------|------|---------|----------
LAN 22|----------|---------|----------|------|---------|----------

### Таблица адресна схема

| Устройство 	| Интерфейс 	| IP aдрес 	| Маска 	| Маршрут по подразбиране/gateway 	|
|------------	|----------:	|----------	|-------	|---------------------------------	|
| ------      | ------    	| ------   	| ------	| ------                          	|
| ------     	| ------    	| ------   	|------ 	| ------                          	|
| ------      | ------    	| ------   	|------ 	| ------                          	|
| ------     	|  ------   	| ------   	|------ 	| ------                          	|

# Домашнее задание к занятию "12.5 Сетевые решения CNI"
Задание 1:  Установка Calico.   
Calico устанавливалась с помощью ansible/kubespray из прошлого домашнего задания.  
 
Настройка политики доступа к hello world:  
Сперва всё запретим   
![2021-10-22_09-42-48](https://user-images.githubusercontent.com/78191008/138410919-250fa40d-e5cc-4f15-b6b4-e2a0a8075030.png)  
И проверим   
![2021-10-22_09-44-04](https://user-images.githubusercontent.com/78191008/138411103-ccc0d3cf-a50a-44d2-9247-ed982d564f83.png)  
А теперь разрешим входящие и исходящие соединения   
![2021-10-22_09-46-04](https://user-images.githubusercontent.com/78191008/138411278-182d9394-b057-4d6f-9625-2e35c9959c10.png)  

Задание 2: изучяем, что запущено по умолчанию.  
Проверим установку Calicoctl.  
![2021-10-22_12-13-10](https://user-images.githubusercontent.com/78191008/138410317-79433560-3371-4f46-bd64-1d9e9640480d.png)  
Запустим комманды по очереди:  
calicoctl get node. Мы получим список всех нод в кластере.  
![2021-10-22_12-30-24](https://user-images.githubusercontent.com/78191008/138412243-34207be5-6c43-4fa9-9798-588eb8bd834b.png)  
calicoctl get ipPool. Мы видим каким образом выделяются IP адреса для подов в кластере.   
![2021-10-22_12-32-23](https://user-images.githubusercontent.com/78191008/138412541-7a4fc747-e87e-4dde-9772-5cd637556b3f.png)  
calicoctl get profile. Мы видим все профили сетевых ресурсов.      
![2021-10-22_12-36-35](https://user-images.githubusercontent.com/78191008/138413147-fefa322f-b524-4eb3-8353-41e4183024f5.png)

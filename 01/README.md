Код тут https://github.com/jaack1/netology-ansible-hw/tree/main/01



1. Попробуйте запустить playbook на окружении из test.yml, зафиксируйте значение, которое имеет факт some_fact для указанного хоста при выполнении playbook.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/1.png)

2. Найдите файл с переменными (group_vars), в котором задаётся найденное в первом пункте значение, и поменяйте его на all default fact.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/2.png)

3. Воспользуйтесь подготовленным (используется docker) или создайте собственное окружение для проведения дальнейших испытаний.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/3.png)

4. Проведите запуск playbook на окружении из prod.yml. Зафиксируйте полученные значения some_fact для каждого из managed host.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/4.png)

5. Добавьте факты в group_vars каждой из групп хостов так, чтобы для some_fact получились значения: для deb — deb default fact, для el — el default fact.
6. Повторите запуск playbook на окружении prod.yml. Убедитесь, что выдаются корректные значения для всех хостов.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/6.png)

7. При помощи ansible-vault зашифруйте факты в group_vars/deb и group_vars/el с паролем netology.
8. Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь в работоспособности.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/8.png)

9. Посмотрите при помощи ansible-doc список плагинов для подключения. Выберите подходящий для работы на control node.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/9.png)

10. В prod.yml добавьте новую группу хостов с именем local, в ней разместите localhost с необходимым типом подключения.
11. Запустите playbook на окружении prod.yml. При запуске ansible должен запросить у вас пароль. Убедитесь, что факты some_fact для каждого из хостов определены из верных group_vars.
![Image alt](https://github.com/jaack1/netology-ansible-hw/blob/main/01/screenshots/11.png)


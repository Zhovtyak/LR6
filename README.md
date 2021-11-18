# LR6
Лабораторная работа №6
1. Форкаем репозиторий на свой профиль
![image](https://user-images.githubusercontent.com/94613997/142414447-6459057d-15f4-4419-9858-9d8c3f74da63.png)
2. Задаем имя пользователя и email </br>
![image](https://user-images.githubusercontent.com/94613997/142414973-eb5b346f-0ad3-48f1-bc95-9caeeadd830d.png)
3. Клонируем удаленный репозиторий на компьютер
![image](https://user-images.githubusercontent.com/94613997/142415125-5aec5733-0eeb-4265-94f3-f6db86adde11.png)
4. Добавляем файл через интерфейс Github
![image](https://user-images.githubusercontent.com/94613997/142415591-08a50631-6b37-405d-8418-5c6f02f430c0.png)
![image](https://user-images.githubusercontent.com/94613997/142416227-5fd8a1af-014b-4ada-977e-69c567167f69.png)
5. Подтягиваем изменения в локальный репозиторий
![image](https://user-images.githubusercontent.com/94613997/142416445-9a817a82-e28c-4aaf-ac76-9502034002fd.png)
6. Получаем историю для каждой ветки
![image](https://user-images.githubusercontent.com/94613997/142416627-5f337dcf-870d-4daf-8e5f-8d8d4f553205.png)
7. Смотрим последние изменения ветки (изменений много, но в качестве примера представил один скриншот)
![image](https://user-images.githubusercontent.com/94613997/142417383-92deeeac-ae45-4aac-b8b7-8a4065dacd22.png)
8. Выполняется слияние и разрешается конфиликт </br>
8.1. Переходим в ветку brunch1 </br>
![image](https://user-images.githubusercontent.com/94613997/142421981-08e56f05-61a7-4095-8b25-8fb21e1c1bce.png)</br>
8.2. Выполняем слияние и получаем сообщение о конфликте</br>
![image](https://user-images.githubusercontent.com/94613997/142422137-8c573eaf-e103-4ce4-9e2f-387ed5f22645.png)</br>
8.3. Выясняем причину конфликта </br>
![image](https://user-images.githubusercontent.com/94613997/142422307-8ca297be-561e-4ea2-80c0-b36fcbc98609.png)</br>
8.4. Исправляем причину конфикта </br>
![2021-11-18_16-05-26](https://user-images.githubusercontent.com/94613997/142422420-530bef40-865b-41cf-aaea-d2aeeae5bc04.png)
![2021-11-18_16-06-11](https://user-images.githubusercontent.com/94613997/142423240-f1ed375e-46ce-4879-b929-7ce59c256d5f.png) </br>
8.5. Добавляем содержимое рабочего каталога в индекс для последующего коммита </br>
![image](https://user-images.githubusercontent.com/94613997/142423460-11812440-0275-40a8-9416-7725208b2128.png) </br>
8.6. Смотрим, исправлена ли ошибка и завершаем merge </br>
![image](https://user-images.githubusercontent.com/94613997/142423768-b9cb19fe-0617-455d-9ad0-db450a77ca33.png)
9. Удаляем побочную ветку master </br>
![image](https://user-images.githubusercontent.com/94613997/142423903-08ae25ed-ece5-4d03-9479-ee827c2a41b9.png)
10. Делаю изменение в файле mergefile.txt и коммичу его, оставляя комментарий
![image](https://user-images.githubusercontent.com/94613997/142425265-77811aaf-9499-4878-b561-39fadbb02fa7.png)
11. Создаю новый файл и коммичу его, оставляя комментарий </br>
![image](https://user-images.githubusercontent.com/94613997/142425537-2c75584e-e01b-479e-a7f1-40342c74847e.png)
12. Делаю хард откат коммита </br>
![image](https://user-images.githubusercontent.com/94613997/142425899-56ea01d6-7e8e-4a4f-9a51-08514d41dd55.png)
13. Создаю ветку для отчета и перехожу на неё </br>
![image](https://user-images.githubusercontent.com/94613997/142427782-c5d31c24-9dc9-40c6-9a5c-973be9ee6b46.png)
14. Отправляю все данные на удаленный репозиторий 
![image](https://user-images.githubusercontent.com/94613997/142428247-ba1bb211-a3b3-4cec-8a86-f67518ba3b27.png)
# Лог команд
git config global user.name/email </br>
git clone https://github.com/Zhovtyak/LR6 </br>
git pull </br>
git reflog --all </br>
git log -p </br>
git checkout branch1 </br>
git merge master </br>
git diff </br>
git add mergefile.txt </br>
git status </br>
git commit -m "Merged" </br>
git branch -d master </br>
git add mergefile.txt </br>
git commit -m "Info updated" </br>
git add WOW.txt </br> 
git commit -m "New file just for fun" </br>
git reset --hard HEAD </br>
git checkout -b otchet </br>
git branch </br>
git push --set-upstream origin otchet </br>
# История операция
commit bdc6b56b4d5975c18068ad48fb53bbb437726759 (HEAD -> otchet, origin/otchet, branch1) </br>
Author: 4016ZhovtyakMO <jasdef124@gmail.com> </br>
Date:   Thu Nov 18 16:37:35 2021 +0300 </br>

    New file just for fun

commit dded87d9a699d86ed9e9c55497cc35f2cf5a1349 </br> 
Author: 4016ZhovtyakMO <jasdef124@gmail.com> </br> 
Date:   Thu Nov 18 16:35:50 2021 +0300 </br>

    Info updated

commit 52ccc499b186bce9e2db96507f87e4dac0d315ee </br>
Merge: 0f9f50d 223eb53 </br>
Author: 4016ZhovtyakMO <jasdef124@gmail.com> </br>
Date:   Thu Nov 18 16:09:51 2021 +0300 </br>

    Merged

commit 223eb5347f60a8716568a624cbba6bb11c318956 (origin/master, origin/HEAD) </br>
Author: Zhovtyak <94613997+Zhovtyak@users.noreply.github.com> </br>
Date:   Thu Nov 18 15:34:05 2021 +0300 </br>

    Create NewFile

commit 921f53b8d0cebf542c791cf31f04e9b792f385a4 </br>
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com> </br>
Date:   Sat Nov 21 20:09:49 2020 +0300 </br>

    Обновление информации

commit 0f9f50db68a6983b47398017545532cd0f992846 (origin/branch1) </br>
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com> </br>
Date:   Sat Nov 21 20:08:33 2020 +0300 </br>

    Заполнил файл

commit c08a654a63cfc3a7146b2b7015884d9020f5cbf5 </br>
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com> </br>
Date:   Sat Nov 21 20:02:16 2020 +0300 </br>

    Файл создан пустым

commit 3c6e9131bb47ed6009c28226afb0535c7f6d5964 </br>
Author: Kurtyanik <45309985+Kurtyanik@users.noreply.github.com> </br>
Date:   Sat Nov 21 19:58:20 2020 +0300 </br>

    Initial commit

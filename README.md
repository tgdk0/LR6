**Отчет по лабораторной работе №6** 

**По курсу: Основы программирования**

**Выполнил студент гр. 4917 В.А. Дорофеев**


**Ход работы:**

На сайте GitHub сделал копию лабораторной работы https://github.com/Kurtyanik/LR6/

![Копированный репозиторий](screenshots/screen1.png)

Далее ввел имя и email пользователя, тем самым настроив клиент

![Персональные данные](screenshots/screen2.png)

С помощью команды _mkdir ~/Desktop/LR6_ перешел на рабочий стол и создал папку LR6, после чего перешел в нее с помощью команды _cd ~/Desktop/LR6_ и инициализировал гит в данной папке посредством _git init_

![git init](screenshots/screen3.png)

Командой _git remote add origin_ связал папку с удаленным репозиторием и командой _git clone_ клонировал удаленный репозиторий на компьютер на сайте GitHub

![git remote add origin](screenshots/screen4.png)

Добавил новый файл file.txt в удаленный репозиторий, в ветку **master**, через интерфейс GitHub

![Новый файл](screenshots/screen5.png)

![Новый файл](screenshots/screen6.png)


Далее, используя команду _git pull origin master_ загрузил изменения из удалённого репозитория в локальный

![git pull](screenshots/screen7.png)


Командой _git log_ получил список коммитов и операций

![git log](screenshots/screen8.png)

Используя _git show_ получил  информацию о последнем изменении

![git show](screenshots/screen9.png)

Командой _git checkout -t branch1_ попытался переключиться на ветку **branch1**, но выдало ошибку. Поэтому обновил подключение к сайту GitHub при помощи команды _git remote update_ и повторил попытку

![git checkout](screenshots/screen10.png)


Далее попытался выполнить слияние веток **master** и **branch1** командой _git merge branch1_, но получил очередную ошибку, заключавшуюся в конфликте в файле **mergefile.txt**

![merge failed](screenshots/screen11.png)

Для ее разрешения вручную изменил содержание файла **mergefile.txt**, устранив ошибку слияния и выполнил коммит

![merge fix](screenshots/screen12.png)

Выполнил слияние веток **master** и **branch1**  с помощью команды _git merge branch1_, затем удалив ветку **branch1** командой _git branch -d branch1_

![Слияние и удаление](screenshots/screen13.png)

Занес всё в удалённый репозиторий командой _git push -f origin master_ 

![Push1](screenshots/screen14.png)

Далее добавил два новых текстовых файла (file2+file3)

![file2, file3](screenshots/screen15.png)

![file2, file3 git log](screenshots/screen16.png)

Командой _git reset --hard HEAD~1_ выполнил откат последнего коммита - добавления файла file3.txt

![hard](screenshots/screen17.png)

После чего занес измененную ветку в удаленный репозиторий

![push](screenshots/screen18.png)

![result](screenshots/screen19.png)

Используя команду _git checkout -b otchet_ создал новую ветку **otchet**

![report](screenshots/screen20.png)

История _git log --graph_. Аргумент _--graph_ позволяет графически изобразить ветки и коммиты на них

![graph log](screenshots/screen21.png)

С помощью команды _git add ._ подготовил все новые файлы в папке LR6 к добавлению и занес в удаленный репозиторий

![git add+status](screenshots/screen22.png)

![git commit+push](screenshots/screen23.png)

Оформил отчёт в файле **README.md**, используя блокнот

![Readme](screenshots/screen24.png)

Лог команд из папки **.git/logs**

![Logs](screenshots/screen25.png)

Конечный результат команды _git log_

![git logs](screenshots/screen26.png)

Все скриншоты лежат в папке **screenshots**
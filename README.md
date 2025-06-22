# Домашнее задание к занятию "`GitLab`" - `Лоскутов Вячеслав`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1:

1. `ГитЛаб был развёрнут без использования Vagrant локально, из установочного пакета, на моём сервере:`

![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/Gitlab.PNG)

3. `ГитЛаб запущен локально, далее создан новый проект и репозиторий:`
   
![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/localrun.PNG)
![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/proj.PNG)

5. `Зарегистрирован gitlab-runner для этого проекта и запущен в режиме Docker:`

![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/runnerreg.PNG)
![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/showrun.PNG)
![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/runnerconf.PNG)

### Задание 2

1. `Запушил репозиторий на GitLab, изменив origin:`

![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/Originss.PNG)
![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/neworigin.PNG)

3. `Создал файл .GitLab-ci.yml:`

`stages:
  - test
  - build

test:
  stage: test
  image: golang:1.17
  script: 
   - go test .

build:
  stage: build
  image: docker:latest
  script:
   - docker build .`

3. `Успешно собранная сборка:`
![alt text](https://github.com/NightWalkerZ488/git-hwork/blob/main/rundone.jpg)


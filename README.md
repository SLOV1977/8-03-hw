# Домашнее задание к занятию "`GitLab`" - `Рахманов Александр`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw.
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

## Решение.

### Задание 1.

![Настройки раннера](https://github.com/SLOV1977/8-03-hw/tree/main/img/8-03-1.png)

![Настройки раннера](img/8-03-1.png)

---

### Задание 2.

![Файл gitlab-ci.yml:](https://github.com/SLOV1977/8-03-hw/tree/main/.gitlab-ci.yml)

```
workflow:
  rules:
    - if: '$CI_COMMIT_BRANCH'
      when: always

stages:
  - verify

verify:
  stage: verify
  image: alpine:latest
  script:
    - echo "Repository with 3 files verified successfully"

```

![Вкладка Pipeline раздела Pipeline сборки](https://github.com/SLOV1977/8-03-hw/tree/main/img/8-03-2.1.png)

![Вкладка Pipeline раздела Pipeline сборки](img/8-03-2.1.png)

---

![Вкладка Jobs раздела Pipeline сборки](https://github.com/SLOV1977/8-03-hw/tree/main/img/8-03-2.2.png)

![Вкладка Jobs раздела Pipeline сборки](img/8-03-2.2.png)

---

![Раздел Jobs сборки](https://github.com/SLOV1977/8-03-hw/tree/main/img/8-03-2.3.png)

![Раздел Jobs сборки](img/8-03-2.3.png)

---
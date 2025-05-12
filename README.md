# Величко Дмитро ІПЗ 3.02
## Практично-лабораторне заняття №8
## Тема: Неперервна інтеграція

# Туторіал
## 1. Завершити наступні практичні роботи на GitHub Skills, надати посилання на репозиторії з виконаним завданням у звіті


# Проходження Hello GitHub Actions

Перейшов за посилання [https://github.com/skills/hello-github-actions?tab=readme-ov-file](https://github.com/skills/hello-github-actions?tab=readme-ov-file) і натиснув кнопку "Start course"

![create_repo](https://github.com/user-attachments/assets/6a123e33-9136-456e-bee0-0e7ebedc4fb9)

Після створення репозиторію. Треба виконати інструкцію яка написана в ```README```.

# Step 1: Create a workflow file

1. Перейти до вкладки ```Pull request``` і створити новий запит (```New pull request```).

![create_pull_request](https://github.com/user-attachments/assets/0a4eeefe-eabd-40fb-967c-d32a884be28f)

Далі натискаємо ```Create pull request```

![open_pull_request](https://github.com/user-attachments/assets/32a0753e-5ec9-4577-8587-f01f62238695)

Тепер, ще раз натискаємо ```Create pull request```

![pull_request_welcome_workflow](https://github.com/user-attachments/assets/424149c2-ab05-4e14-9a58-7d5a4579d027)

2. Після цього натискаємо вкладку код (```Code```). Після цього у випадаючому вікні замінюємо ```main``` на ```welcome-workflow```.

![main_welcome-workflow](https://github.com/user-attachments/assets/dfb4371d-c724-4697-8e3d-0bbd9fc6be23)

3. Після цього переходимо за таким шляхом ```.github/workflows/``` потім натискаємо ```Add file->Create new file```. І надаємо назву файлу: ```welcome.yml```.
4. Тепер у цьому файлі додаємо такий вміст:

![welcome_yml_content](https://github.com/user-attachments/assets/6fc136e1-b099-4eda-b7e2-778d66123ee1)

5. Тепер зберігаємо зміни, натиснувши ```Commit changes```. Тепер вибераємо пункт ```Commit directly to the "welcome-workflow" branch``` і натискаємо ```Commit changes```.

![commit_changes](https://github.com/user-attachments/assets/b0ed7ee0-6e11-4a7a-ae88-92802ef4441c)

Тепер переходимо до другого пункту

# Step 2: Add a job to your workflow file

1. Перш за все подивимось чи знаходимось ми у гілці ```welcome-workflow```. Якщо так то ідемо далі.

Тепер перейдемо за напрямом ```.github/workflows/welcome.yml``` і змінемо його вміст.

![change_welcome_yml](https://github.com/user-attachments/assets/5c7596a1-1692-4cf5-99ee-2479d23e4032)

2. Тепер зберігаємо наші зміни.

![update_welcome_yml](https://github.com/user-attachments/assets/72382336-06b6-43ca-b737-f1e50fe7d3e7)

# Step 3: Add a step to your workflow file

1. Знову переходимо за напрямом ```.github/workflows/``` і знову змінюємо зміст файлу. При цьому ми працюємо у гілці ```welcome-workflow```.

![change_2_welcome_yml](https://github.com/user-attachments/assets/d0d3546d-29a3-4810-8954-255f7ff1ed2d)

Зберігаємо наші зміни, все як і у минулих кроках.

# Step 4: Merge your workflow file
1. Натиснемо на вкладку ```Pull request```.

![pull_request_welcome_workflow_union](https://github.com/user-attachments/assets/06d0f84f-2560-4e28-88fc-4a018cd9d33c)

Тепер натискаємо на запит і натискаємо ```Merge pull request```.

![merge_pull_request](https://github.com/user-attachments/assets/a825f0c1-631f-45fe-b59c-0a984373974e)

Тепер натискаємо ```Confirm merge```

![confirm_merge](https://github.com/user-attachments/assets/457c6b90-c927-456e-81d1-8366ba328fd7)

# Step 5: Trigger the workflow
1. Cтворимо нову гілку ```test-workflow```.

![create_test_workflow_branch](https://github.com/user-attachments/assets/93624fb9-c8c1-4857-b0e8-f3257a5109ff)

2. Після створення зробимо зміну у файлі ```README.md```, нехай додамо смайли.

![change_readme](https://github.com/user-attachments/assets/5c4c2009-6a24-41f0-8d5c-97bae289f548)

Тепер зберігаємо зміни саме на нашій ```НОВІЙ ГІЛЦІ```.

3. Перейдемо у вкладку ```Pull request```

![test_workflow_request](https://github.com/user-attachments/assets/e11a1668-4ea0-4163-8061-d0827273ae95)

І натиснемо на ```Compare & pull request```

![pull_request_test_workflow_and_main](https://github.com/user-attachments/assets/a301e090-0d99-4b31-aeaf-bf8ef001e79e)

І тепер натискаємо ```Create pull request```.

![update_readme](https://github.com/user-attachments/assets/b5ea6363-38f2-4feb-9a8e-c2c5a2dcca96)

І тепер натискаємо ```Merge pull request```.

На цьому закінчується туторіал.

Посилання: [https://github.com/dima2005-gif/skills-hello-github-actions/tree/main](https://github.com/dima2005-gif/skills-hello-github-actions/tree/main)

# Проходження Publish Packages

1. Перейшовши за посиланням натиснув кнопку ```"Start course"```.

Далі було створено репозиторій ```skills-publish-packages```.

# Step 1: Create the workflow file

1. Перемкнемось на іншу гілку, а саме на ``cd``.
2. Перейдемо за шляхом ```.github/workflows/``` і створюємо новий файл з назвою `publish.yml`.
Далі заповнимо його 

Замість `YOURNAME` треба вставити свій `username`, у моєму випадку `Dmytro`.

Тепер зберігаємо зміни натиснувши `Commit changes`.

# Step 2: Add a Dockerfile
1. Перевіримо, що ми знаходимось на гілці cd, якщо так то ідемо далі.
2. Створимо наш Dockerfile у корені проекту і додамо такий зміст:

![create_dokerfile](https://github.com/user-attachments/assets/c0c6c3eb-57bd-4729-89e5-6c08f3661563)

Зберігаємо наші зміни.

# Step 3: Merge your changes
1. Тепер перейдемо до вкладки `Pull request` і об'єднаємо гілки.

Для цього натиснемо `Create pull request`

![pull_request_cd_main](https://github.com/user-attachments/assets/c01a4588-5a8b-46f9-badd-55b0d57e90da)

Тепер натискаємо `Merge pull request`.

# Step 4: Pull your image
1. Так як у мене стоїть Docker то ми можемо працювати далі. Перейдемо у налаштування і створемо новий токен класичний

Тепер нам видає таке вікно:

![create_token_content](https://github.com/user-attachments/assets/f159cd4c-9beb-467a-98c1-d3fe291a9fd5)

Надаємо назву наприклад `"GitHub Packages deploy"`.

Так тепер відкриємо наш термінал. Пишемо команду: `docker login ghcr.io -u USERNAME`

Замість `USERNAME` напишемо наше ім'я, у нашому випадку `Dmytro`.

Пароль використовуємо персональний токен.

Результат:

![login_succeeded](https://github.com/user-attachments/assets/3714acb7-ac01-461e-9028-fecdb2b60018)

Так перейдемо у вкладку `Package` і там буде наш `image`

![package](https://github.com/user-attachments/assets/d7c95cd2-a70d-4a12-bb57-9d46f382417b)

Тепер у терміналі вставимо команду для встановлення `image`

![comand_image](https://github.com/user-attachments/assets/c7a12ec7-a81c-41a6-b93a-0c3b1378f77f)

# Step 5: Run your image

Переглянемо зміст image за допомогою команди `docker image ls`

![docker_image_ls](https://github.com/user-attachments/assets/76256b98-c42e-48ba-926e-4b811d54cbcb)

Так тепер запустимо наш контейнер за допомогою команди: `docker run -dp 8080:80 --rm <YOUR_IMAGE_NAME:TAG>`

- Замініть `YOUR_IMAGE_NAME` назву зображення під `REPOSITORY` стовпцем.
- Замініть `TAG` тегом зображення під `TAG` стовпцем.

У нашому випадку:
- `YOUR_IMAGE_NAME` = `ghcr.io/dima2005-gif/publish-packages/game`
- `TAG` = `sha-0aacd34`

![docker_run](https://github.com/user-attachments/assets/305181f0-ebf3-48a2-985d-7f9de0f0e6f5)

На цьому туторіал закінчився.

# Лабораторна
1. По перше запушимо нашу 7 лабораторну роботу. Для цього виконаємоо команди:

`git init`

потім 

`git remote add origin https://github.com/dima2005-gif/KPZ_lb_pr_8.git`

далі

`git add .`

і нарешті

`git commit -m "Запушил лабораторную работу"`

Тепер глянемо на наш репозиторій і бачимо:

![check_repo](https://github.com/user-attachments/assets/50c24255-8cfa-4567-9502-78e8a4d570b8)

2. Створемо каталог `.github`, а у ньому ще такий каталог `workflows`, а у ньому створемо файл `docker-build.yml`

![create_workflow_lb_8](https://github.com/user-attachments/assets/0199666a-357d-4222-a80f-54c826467600)


Зберігаємо зміни, натиснувши кнопку `Commit change`. Потім перейдемо у вкладку `Actions` і побачимо, що:

![action_check](https://github.com/user-attachments/assets/89173dfa-1db1-436a-9669-e9ff8824fd84)

Усе удачно і наш воркфлоу працює.

Тепере перейдемо у вкладку `Packages` і побачимо, що:

![packeges_check](https://github.com/user-attachments/assets/353d918b-bd9c-4c86-952d-9de354a84db5)

у нас з'явився докер екземпляр.

## Практично-лабораторне заняття №9
## Тема: Неперервна доставка

1.Перейдемо у `Microsoft Azure`, у полі пошуку пишемо `"App Servces"` і натискаємо кнопку `Create` і вибераємо `Web App`. 

І нам відкривається вікно:

![create_web_app](https://github.com/user-attachments/assets/ade38384-4c4e-4c14-b487-73e2db243a04)

І тепер заповнюємо пункти відповідно значенням:

- `Resource Group` натискаємо `Create new` і пишемо наприклад `kpz`
- `Name` пишемо наприклад `myapp-lb9`
- В `Publish` вибераємо `Container`
- `Region` вибераємо `West Europe`
- Далі `Pircing plan` тут ми вибераємо `Free F1`

і далі натискаємо кнопку `Review+create`. І далі натискаємо `Create`.

2. Так тепер ми можемо ідти далі. Створимо у `Azure Service`, `principal`.

Для цього натиснемо на кнопку терміналу

![terminal](https://github.com/user-attachments/assets/8dc70f3e-e491-4e6c-acf1-4e19c0f1a523)

Так тепер введемо команду: 

`az ad sp create-for-rbac --name "myApp" --role contributor --scopes /subscriptions/<subscription_id>/resourceGroups/<resource_group_name> --json-auth`

Замінивши  `<subscription_id>` на `Subscription ID`

![subscription_id](https://github.com/user-attachments/assets/2a8612a1-35f2-4de1-a91a-1ba61eb22942)

А `<resource_group_name>` на назву з `Resource groups`

![resource_group_name](https://github.com/user-attachments/assets/b4ba713c-1cb9-4dcf-9452-34272219b2e6)


і тепер натискаємо Enter і нам термінал видасть на кшталт такого:
```
{
  "clientId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "clientSecret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "subscriptionId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "tenantId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "activeDirectoryEndpointUrl": "...",
  "resourceManagerEndpointUrl": "...",
  (...)
}
```

Так-с тепер скопіюємо це.

3. Створимо секрет. Перейдемо у GitHub у наш репозиторій і за таким шляхом

`settings -> secrets and variables -> actions`, та натиснемо `New Repository Secret`. В полі `Name`
введемо `AZURE_CREDENTIALS` а в поле `Secret` вставимо:

```
{
  "clientId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "clientSecret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "subscriptionId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "tenantId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "activeDirectoryEndpointUrl": "...",
  "resourceManagerEndpointUrl": "...",
  (...)
}
```

Тепер натискаємо `Add Secret`.

![secret](https://github.com/user-attachments/assets/ea00b353-c0f5-40fb-91f1-d620f9406f09)


5. Так тепер перейдемо у наш воркфлоу, за шляхом `.github/workflows/docker-build.yml`.

І тепер додамо пару рядків.

![add_docker_build](https://github.com/user-attachments/assets/21dbe225-46bf-413d-969d-0f12354033b7)

Зберігаємо наші зміни `Commit change`. І тепер перевіримо роботу нашого воркфлоу.

Перейдемо у вкладку `Actions` і побачимо: 

![actions_check](https://github.com/user-attachments/assets/b635d0d6-73d4-4df2-b419-9cbc0e2dfc5c)

Як бачимо усе працює.

7. Тепер перевіремо наш деплой. Для цього перейдемо у наш воркфлоую.
І натиснемо у вкладці `Jobs 'build-and-push'`, і натискаємо на 
`Deploy to Azure Web App`

![deploy_check](https://github.com/user-attachments/assets/032942e0-cd58-4ff8-8850-3a1dabc936c9)

І натискаємо на посилання. І...

![finish](https://github.com/user-attachments/assets/382c3881-3297-454f-a4d6-201a772fb7b3)

Усе добре, усе відображається. Отже, усе у нас нормально.

# Висновок
У ході виконання лабораторно-практичних занять №8 і №9 я ознайомився з принципами та основними практиками неперервної інтеграції (CI) і неперервної доставки (CD) 
на прикладі GitHub Actions та Microsoft Azure.
Пройшовши практичні курси Hello GitHub Actions та Publish Packages, де навчився:
- створювати CI-процеси за допомогою YAML-файлів;
- автоматично запускати дії при зміні коду в репозиторії;
- створювати Docker-образи та публікувати їх у GitHub Packages;
- запускати створені Docker-контейнери локально через термінал.

У лабораторній частині:
- було створено власний GitHub Actions workflow (docker-build.yml) для автоматичного складання Docker-образу з коду проєкту;
- налаштував зберігання та публікацію образу в GitHub Packages;
- реалізував автоматичний деплой Docker-контейнера у хмарну платформу Microsoft Azure Web App за допомогою секретів і сервісного принципала.

Отже, я отримав практичні навички налаштування автоматизованих CI/CD процесів, що є важливим етапом у розробці сучасного програмного забезпечення. Ці знання дозволяють забезпечити стабільність, повторюваність та швидке розгортання застосунків у продакшн-середовище.


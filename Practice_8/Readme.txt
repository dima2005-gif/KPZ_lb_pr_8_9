Практично-лабораторне заняття №8
Тема: Неперервна інтеграція
Мета: ознайомитися з принципами і практиками 
неперервної інтеграції, сформувати навички 
автоматизації CI/CD процесів в GitHub Actions

Туторіал

1.Завершити наступні практичні роботи на GitHub Skills, надати посилання на 
репозиторії з виконаним завданням у звіті
Проходження Hello GitHub Actions
Перейшов за посилання і натиснув кнопку "Start course"
create_repo.png
Після створення репозиторію. Треба виконати інструкцію яка написана в README.
1. Перейти до вкладки Pull request і створити новий запит (New pull request).
create_pull_request.png
Далі натискаємо Create pull request
open_pull_request.png
Тепер, ще раз натискаємо Create pull request
pull_request_welcome_workflow.png
2. Після цього натискаємо вкладку код (Code). Після цього у випадаючому вікні 
замінюємо main на welcome-workflow.
main_welcome-workflow.png
3. Після цього переходимо за таким шляхом .github/workflows/
потім натискаємо Add file->Create new file. І надаємо назву файлу: welcome.yml.
4. Тепер у цьому файлі додаємо такий вміст:
welcome_yml_content.png
5. Тепер зберігаємо зміни, натиснувши Commit changes.
Тепер вибераємо пункт Commit directly to the "welcome-workflow" branch і натискаємо 
Commit changes.
commit_changes.png
Тепер переходимо до другого пункту
Step 2: Add a job to your workflow file
1. Перш за все подивимось чи знаходимось ми у гілці welcome-workflow. Якщо так то ідемо далі.
Тепер перейдемо за напрямом .github/workflows/welcome.yml і змінемо його вміст.
change_welcome_yml.png
2. Тепер зберігаємо наші зміни.
update_welcome_yml.png
Step 3: Add a step to your workflow file
1. Знову переходимо за напрямом .github/workflows/ і знову змінюємо зміст файлу.
При цьому ми працюємо у гілці welcome-workflow.
change_2_welcome_yml.png
Зберігаємо наші зміни, все як і у минулих кроках.
Step 4: Merge your workflow file
1. Натиснемо на вкладку Pull request. 
pull_request_welcome_workflow_union.png
Тепер натискаємо на запит і натискаємо Merge pull request.
merge_pull_request.png
Тепер натискаємо Confirm merge
confirm_merge.png
Step 5: Trigger the workflow
1. Cтворимо нову гілку test-workflow. 
create_test_workflow_branch.png
2. Після створення зробимо зміну у файлі README.md, нехай додамо смайли.
change_readme.png
Тепер зберігаємо зміни саме на нашій НОВІЙ ГІЛЦІ.
3. Перейдемо у вкладку Pull request 
test_workflow_request
І натиснемо на Compare & pull request
pull_request_test_workflow_and_main.png
І тепер натискаємо Create pull request.
update_readme.png
І тепер натискаємо Merge pull request.
На цьому закінчується туторіал.
Посилання: https://github.com/dima2005-gif/skills-hello-github-actions/tree/main

Проходження Publish Packages
1. Перейшовши за посиланням натиснув кнопку "Start course".
Далі було створено репозиторій skills-publish-packages.
Step 1: Create the workflow file
1. Перемкнемось на іншу гілку, а саме на cd.
main_switch_cd.png
2. Перейдемо за шляхом .github/workflows/ і створюємо новий файл з назвою publish.yml.
Далі заповнимо його таким змістом:
create_and_content_publish_yml.png
Замість YOURNAME треба вставити свій username, у моєму випадку Dmytro.\
Тепер зберігаємо зміни натиснувши Commit changes.

Step 2: Add a Dockerfile
1. Перевіримо, що ми знаходимось на гілці cd, якщо так то ідемо далі.
2. Створимо наш Dockerfile у корені проекту і додамо такий зміст:
create_dokerfile.png
Зберігаємо наші зміни.

Step 3: Merge your changes
1. Тепер перейдемо до вкладки Pull request і об'єднаємо гілки.
Для цього натиснемо Create pull request
pull_request_cd_main.png
Тепер натискаємо Merge pull request.

Step 4: Pull your image
1. Так як у мене стоїть Docker то ми можемо працювати далі.
Перейдемо у налаштування і створемо новий токен класичний
create_token.png
Тепер нам видає таке вікно:
create_token_content.png
Надаємо назву наприклад "GitHub Packages deploy".
Так тепер відкриємо наш термінал. Пишемо команду: docker login ghcr.io -u USERNAME
Замість USERNAME напишемо наше ім'я, у нашому випадку Dmytro.
Пароль використовуємо персональний токен.
Результат:
login_succeeded.png

Так перейдемо у вкладку Package і там буде наш image
package.png
Тепер у терміналі вставимо команду для встановлення image
comand_image.png

Step 5: Run your image
Переглянемо зміст image за допомогою команди docker image ls
docker_image_ls.png
Так тепер запустимо наш контейнер за допомогою команди: docker run -dp 8080:80 --rm <YOUR_IMAGE_NAME:TAG>
Замініть YOUR_IMAGE_NAME назву зображення під REPOSITORY стовпцем.
Замініть TAG тегом зображення під TAG стовпцем.
У нашому випадку 
YOUR_IMAGE_NAME = ghcr.io/dima2005-gif/publish-packages/game
TAG = sha-0aacd34
docker_run.png
На цьому туторіал зацінчився.


Лабораторна
1. По перше запушимо нашу 7 лабораторну роботу. Для цього 
виконаємоо команди:
git init
потім 
git remote add origin https://github.com/dima2005-gif/KPZ_lb_pr_8.git
далі
git add .
і нарешті
git commit -m "Запушил лабораторную работу"
Тепер глянемо на наш репозиторій і бачимо:
check_repo.png

2. Створемо каталог .github, а у ньому ще такий каталог workflows, 
а у ньому створемо файл docker-build.yml 
create_workflow_lb_8.png
Зберігаємо зміни, натиснувши кнопку Commit change. Потім перейдемо у вкладку Actions
і побачимо, що:
action_check.png
Усе удачно і наш воркфлоу працює.
Тепере перейдемо у вкладку Packages і побачимо, що:
packeges_check.png
у нас з'явився докер екземпляр.
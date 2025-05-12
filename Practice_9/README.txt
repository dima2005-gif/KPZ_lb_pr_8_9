Лабораторна-практична робота № 9
Тема: Неперервна доставка
1.Перейдемо у Microsoft Azure, у полі пошуку пишемо
"App Servces" і натискаємо кнопку Create і вибераємо Web App. 
І нам відкривається вікно:
create_web_app.png
І тепер заповнюємо пункти відповідно значенням:
Resource Group натискаємо Create new і пишемо наприклад kpz
Name пишемо наприклад myapp-lb9
В Publish вибераємо Container
Region вибераємо West Europe
Далі Pircing plan тут ми вибераємо Free F1
і далі натискаємо кнопку Review+create. І далі натискаємо Create.
2. Так тепер ми можемо ідти далі. Створимо у Azure Service, principal.
Для цього натиснемо на кнопку терміналу
terminal.png
Так тепер введемо команду: az ad sp create-for-rbac --name "myApp" --role contributor --scopes /subscriptions/<subscription_id>/resourceGroups/<resource_group_name> --json-auth
Замінивши  <subscription_id> на Subscription ID
subscription_id.png
А <resource_group_name> на назву з Resource groups
resource_group_name.png
і тепер натискаємо Enter і нам термінал видасть на кшталт такого:
{
  "clientId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "clientSecret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "subscriptionId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "tenantId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "activeDirectoryEndpointUrl": "...",
  "resourceManagerEndpointUrl": "...",
  (...)
}
Так-с тепер скопіюємо це.
3. Створимо секрет. Перейдемо у гітхаб у наш репозиторій і за таким шляхом
settings -> secrets and variables -> actions, та натиснемо New Repository Secret. В полі Name
введемо AZURE_CREDENTIALS а в поле Secret вставимо:
{
  "clientId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "clientSecret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "subscriptionId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "tenantId": "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
  "activeDirectoryEndpointUrl": "...",
  "resourceManagerEndpointUrl": "...",
  (...)
}
Тепер натискаємо Add Secret.
secret.png
4. Так тепер перейдемо у наш воркфлоу, за шляхом .github/workflows/docker-build.yml.
І тепер додамо пару рядків.
add_docker_build.png
Зберігаємо наші зміни Commit change. І тепер перевіримо роботу нашого воркфлоу.
Перейдемо у вкладку Actions і побачимо: 
actions_check.png
Як бачимо усе працює.
5. Тепер перевіремо наш деплой. Для цього перейдемо у наш воркфлоую.
І натиснемо у вкладці Jobs 'build-and-push', і натискаємо на 
Deploy to Azure Web App
deploy_check.png
І натискаємо на посилання. І...
finish.png
Усе добре, усе відображається. Отже, усе у нас нормально.

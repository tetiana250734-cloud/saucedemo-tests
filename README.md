# saucedemo-tests
saucedemo-tests (testing logo)
# Ініціалізація локального репозиторію
git init
# Додавання всіх файлів
git add .
# Перший коміт
git commit -m "Initial commit: базова структура проєкту"
# Підключення до GitHub/GitLab
git remote add origin <url-репозиторію>
# Відправка у головну гілку
git branch -M main
git push -u origin main
# Створити нову гілку
git checkout -b setup-wdio
# Зробити зміни (наприклад, ініціалізація WebdriverIO)
git add .
git commit -m "Setup WebdriverIO project"
# Відправити гілку на GitHub
git push origin setup-wdio

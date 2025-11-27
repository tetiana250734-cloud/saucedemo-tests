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
1)	git checkout -b page-objects
# додати LoginPage.js, InventoryPage.js 
git commit -m "Add Page Object files"
git push origin page-objects
2)	git checkout -b login-tests
# додати login.spec.js
git checkout -b cart-tests
# додати cart.spec.js
git commit -m "Automated cart tests"
git push origin cart-tests
git checkout -b checkout-tests
# додати checkout.spec.js
git commit -m "Automated checkout tests"
git push origin checkout-tests
git checkout -b sorting-tests
# додати sorting.spec.js
git commit -m "Automated sorting tests"
git push origin sorting-tests
git checkout -b logout-tests
# додати logout.spec.js
git commit -m "Automated logout tests"
git push origin logout-tests
git status       # показує зміни
git branch       # показує всі гілки
git log --oneline # історія комітів
# додати злиття гілок
git branch -d setup-wdio
git push origin --delete setup-wdio

git commit -m "Automated login tests"
git push origin login-tests

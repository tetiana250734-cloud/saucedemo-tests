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

chore: initial commit with project structure
docs: add README.md with project overview
setup: initialize WebdriverIO with npm init wdio
chore: configure wdio.conf.js with baseUrl
test: add sample test from init setup
feat: add LoginPage object with login method
feat: add InventoryPage object with add to cart method
feat: add CartPage object with checkout navigation
feat: add CheckoutPage object with form fields
test: implement login.spec.js with positive case
test: add negative login tests (locked_out_user, empty fields)
refactor: improve error message selector in LoginPage
test: implement cart.spec.js with add/remove tests
test: verify cart badge updates correctly
refactor: reuse InventoryPage methods in cart tests
test: implement checkout.spec.js with successful checkout
test: add validation tests for missing fields
refactor: optimize CheckoutPage selectors
test: add sorting.spec.js with price low→high
test: add sorting.spec.js with price high→low
test: add sorting.spec.js with name A→Z and Z→A
test: implement logout.spec.js
refactor: add logout method in InventoryPage
test: verify product images are displayed
test: check product prices are correct
test: validate error messages for invalid checkout

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
git checkout -b main
git commit --allow-empty -m "chore: initial commit with project structure"
git add README.md
git commit -m "docs: add README.md with project overview"
git push origin main
git checkout -b setup-wdio
npm init wdio
git add wdio.conf.js
git commit -m "setup: initialize WebdriverIO with npm init wdio"
git commit -m "chore: configure wdio.conf.js with baseUrl"
git add test/sample.e2e.js
git commit -m "test: add sample test from init setup"
git push origin setup-wdio
git checkout -b page-objects
git add LoginPage.js InventoryPage.js CartPage.js CheckoutPage.js
git commit -m "feat: add LoginPage object with login method"
git commit -m "feat: add InventoryPage object with add to cart method"
git commit -m "feat: add CartPage object with checkout navigation"
git commit -m "feat: add CheckoutPage object with form fields"
git push origin page-objects
git checkout -b login-tests
git add login.spec.js
git commit -m "test: implement login.spec.js with positive case"
git commit -m "test: add negative login tests (locked_out_user, empty fields)"
git commit -m "refactor: improve error message selector in LoginPage"
git push origin login-tests
git checkout -b cart-tests
git add cart.spec.js
git commit -m "test: implement cart.spec.js with add/remove tests"
git commit -m "test: verify cart badge updates correctly"
git commit -m "refactor: reuse InventoryPage methods in cart tests"
git push origin cart-tests
git checkout -b checkout-tests
git add checkout.spec.js
git commit -m "test: implement checkout.spec.js with successful checkout"
git commit -m "test: add validation tests for missing fields"
git commit -m "refactor: optimize CheckoutPage selectors"
git push origin checkout-tests
git checkout -b sorting-tests
git add sorting.spec.js
git commit -m "test: add sorting.spec.js with price low→high"
git commit -m "test: add sorting.spec.js with price high→low"
git commit -m "test: add sorting.spec.js with name A→Z and Z→A"
git push origin sorting-tests
git checkout -b logout-tests
git add logout.spec.js
git commit -m "test: implement logout.spec.js"
git commit -m "refactor: add logout method in InventoryPage"
git push origin logout-tests 
git checkout -b extra-tests
git add extra.spec.js
git commit -m "test: verify product images are displayed"
git commit -m "test: check product prices are correct"
git commit -m "test: validate error messages for invalid checkout"
git push origin extra-tests

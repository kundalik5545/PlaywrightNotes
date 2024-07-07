
# Playwrigth with JavaScript

It is a Automation tool for web application and mobile app

## Software required :-

1. Node Js
2. Vs code
3. Playwrigth Test for vs code

## VS Code Extension

1. ESLint
2. Prettier
3. ES7 Snipet

## VS Code Font Family

1. roboto Mono
2. Inconsolata
3. Cascadia Code
4. Fira Code
5. Source Code Pro

## Folder Structure :-

1. playwright.config.ts80
2. package.json
3. package-lock.json
4. tests/
 a. example.spec.ts

5. tests-examples/
 a. demo-todo-app.spec.ts
6. package.lock.json
7. package.json
8. playwright.config.js

## Resources to learn

[Medium Article on TDD + Playwright]( https://medium.com/@oroz.askarov/building-a-robust-automation-framework-in-playwright-typescript-version-b13be4e4bf56 ){: .btn}

[PlayList 01](https://www.youtube.com/watch?v=IB2P1FBXjcQ&list=PLhW3qG5bs-L9sJKoT1LC5grGT77sfW0Z8&index=2){: .btn } 

[Playlist 02](https://www.youtube.com/@rajatt95/playlists){: .btn}

[Playlist 03](https://www.youtube.com/playlist?list=PLFGoYjJG_fqrjcgRUcc2ubbZGtbRcC6W8){: .btn}

[Github Framework Repo 01](https://github.com/JayKishoreDuvvuri/Playwright-JavaScript-SauceDemo){: .btn}

[Github Framework Repo 02](https://github.com/rajatt95/TestAutomationFramework_YT_Rajat_Web_Playwright_JS?tab=readme-ov-file){: .btn}

[Demo Practice site](https://www.saucedemo.com/v1/inventory.html){: .btn}

## Folde structure for Automation Project

### C# folder structure

```java
|-- Base Class
|-- Common Utility Class
|-- POM Class
|-- Reports
|-- Screenshots
|-- Test Data
|-- Tests
|-- App.config
|-- using.cs
```

### Playwright folder structure 01

```java
|-- .github
|     |-- workflows
|          |-- 01_ui_tests_chrome.yml
|          |-- 02_ui_tests_select_one.yml.yml
|          |-- 03_ui_tests_ALL.yml
|-- pages
|     |-- BasePage.js
|     |-- CartPage.js
|     |-- Components.js
|     |-- LoginPage.js
|     |-- ProductsPage.js
|-- test-data
|     |-- login_credentials.json
|-- tests-saucedemo
|     |-- components.spec.js
|     |-- login.spec.js
|-- utils
|     |-- VerificationUtils.js
|     |-- WaitUtils.js
|-- .gitignore
|-- package.json
|-- playwright.config.js
```

### Playwright folder structure 02

```javascript
|-- data
    |-- user.json
|-- pageobjects
    |-- loginPage.js
    |-- homePage.js
    |-- productPage.js
    |-- logOutPage.js
|-- pages
    |-- basePage.js
    |-- loginPage.js
    |-- productPage.js
    |-- logOutPage.js
|-- playwright-report
    |-- index.html
|-- testFixtures
    |-- fixture.js
|-- tests
    |-- TC_01_loginPage.test.js
    |-- TC_02_logoutPage.test.js
    |-- TC_03_productPage.test.js
|-- .gitignore
|-- .gitlab-ci.yml
|-- .prettierrc
|-- CustomReporter.js
|-- README.md
|-- config.js
|-- package-lock.json
|-- package.json
|-- playwright.config.js
|-- results.xml
```

### Playwright.config.js

All testing configuration are stored here.

## Important facts

1. We can run test in headless and headed mode just add

* To run in headed mode

```javascript
headless : false
```

* To run in headless

```javascript
headless : true
```

1. We can run test in parallel way

* To run in parallel mode

```javascript
parallel : false
```

* To not run in parallel mode

```javascript
parallel : true
```

## Commonly used terminology

1. require :-
2. async /await
3. package
4. expeect

## Locators in Playwright

1. By Role

```javascript
await page.getByRole('link', {name: 'value'}).click);
```

1. By Role

```javascript
await page.getByLapel(value',{exact : true}).fill('value');
```

1. By Alt Text

```javascript
await page.getByAltText('text').click();
```

1. By Test Id

```javascript
await page.getByTestld.('value').fill('testers talk');
```

1. By Text

```javascript
await page.getByText.('any text').click();
```

```javascript
await page.getByText.('any text',{exact:true}).click();
```

1. By Title

```javascript
await page.getByTitle.('value').click();
```

1. By Xpath Selector

```javascript
 await page.locator ("xpath=//*[@attr='value']"). click();
```

1. By CSS Selector

```javascript
 await page.locator ("css=//*[@attr='value']"). click();
```

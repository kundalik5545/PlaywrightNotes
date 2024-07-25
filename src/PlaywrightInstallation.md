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

[Medium Article on TDD + Playwright](https://medium.com/@oroz.askarov/building-a-robust-automation-framework-in-playwright-typescript-version-b13be4e4bf56)

[PlayList 01](https://www.youtube.com/watch?v=IB2P1FBXjcQ&list=PLhW3qG5bs-L9sJKoT1LC5grGT77sfW0Z8&index=2)

[Playlist 02](https://www.youtube.com/@rajatt95/playlists)

[Playlist 03](https://www.youtube.com/playlist?list=PLFGoYjJG_fqrjcgRUcc2ubbZGtbRcC6W8)

[PlayList 04](https://www.youtube.com/playlist?list=PL6flErFppaj0iQG2_Dd72Jz0bfrzZwMZH)

[Global file setup and cookies use](https://www.youtube.com/watch?v=Gzlhmg-x1_0)

[Github Framework Repo 01](https://github.com/JayKishoreDuvvuri/Playwright-JavaScript-SauceDemo)

[Github Framework Repo 02](https://github.com/rajatt95/TestAutomationFramework_YT_Rajat_Web_Playwright_JS?tab=readme-ov-file)

[LinkedIn Playwright folder structure](https://www.linkedin.com/pulse/building-playwright-javascript-framework-page-object-model-appmetry)

[Demo Practice site](https://www.saucedemo.com/v1/inventory.html)

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

- To run in headed mode

```javascript
headless: false;
```

- To run in headless

```javascript
headless: true;
```

1. We can run test in parallel way

- To run in parallel mode

```javascript
parallel: false;
```

- To not run in parallel mode

```javascript
parallel: true;
```

## Commonly used terminology

1. require :-
2. async /await
3. package
4. expeect

## Locating ELements in Playwright

1. Property
2. CSS
3. Xpath

## Locator finding tools

1. Selectors Hub
2. Chrome dev tool
3. Playwright Build in

## Types of Locators

| Locator                   | Info                                                                                          |
| ------------------------- | --------------------------------------------------------------------------------------------- |
| 1.page.getByRole()        | to locate by explicit and implicit accessibility attributes.                                  |
| 2. page.getByText()       | to locate by text content.                                                                    |
| 3. page.getByLabel()      | to locate a form control by associated label's text.                                          |
| 4.page.getByPlaceholder() | to locate an input by placeholder.                                                            |
| 5. page.getByAltText()    | to locate an element, usually image, by its text alternative.                                 |
| 6. page.getByTitle()      | to locate an element by its title attribute.                                                  |
| 7. page.getByTestId()     | to locate an element based on its data-testid attribute (other attributes can be configured). |

## Locators

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
await page.getByAltText("text").click();
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
await page.locator("xpath=//*[@attr='value']").click();
```

1. By CSS Selector

```javascript
await page.locator("css=//*[@attr='value']").click();
```

## Locator Methods

### Link / Button

```javascript
await page.locator("locator").click();
```

```javascript
await page.click("locator");
```

### Input Box

```javascript
await page.locator("locator").fill("value");
```

```javascript
await page.locator("locator").type("value");
```

```javascript
await page.fill("locator", "value");
```

```javascript
await page.type("locator", "value");
```

### Locate multiple web elements

```javascript
const links = await page.$$("locator");
```

## Writting first test cases

JavaScript is a asynchronous language

1. Each step is independen on other step
2. All step execution happen in parallel way

But in case of automation testing all step are dependent of each other so we need to specify async infrot of each function which return a promise for every function. Also infront of every step we need to specify await so it can wait for element to load.

```javascript
test("Home Page", async ({ page }) => {
  await page.goto("https://demoqa.com/");
});
```

## Playwright Test Case Writting

1. test => To declare test case
2. expect => To write assertions

```javascript
import { test, expect } from "@playwright/test";

test("basic test", async ({ page }) => {
  await page.goto("https://playwright.dev/");
  const name = await page.innerText(".navbar__title");
  expect(name).toBe("Playwright");
});
```

## Test case writting format

- test('title', body)
- test('title', details, body)

## Tags in test case

tag always start with @ and give inside { tag: @smoke,}

```javascript
import { test, expect } from "@playwright/test";

test(
  "basic test",
  {
    tag: "@smoke",
  },
  async ({ page }) => {
    await page.goto("https://playwright.dev/");
    // ...
  }
);
```

## Waits in Javascript with Playwright

| Method                           | Description                                     | Code                                                                                                                      |
| -------------------------------- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Wait for Element to be Visible   | Waits until the element is visible              | await page.waitForSelector('selector', { state: 'visible' });                                                             |
| Wait for Element to be Clickable | Waits until the element is enabled              | await page.waitForSelector('selector', { state: 'enabled' });                                                             |
| Wait for Element to be Hidden    | Waits until the element is hidden               | await page.waitForSelector('selector', { state: 'hidden' });                                                              |
| Wait for Element to Contain Text | Waits until the element contains specified text | await page.waitForSelector('selector', { text: 'expected text' });                                                        |
| Wait for a Specific Timeout      | Waits for a specific amount of time             | await page.waitForTimeout(5000); // waits for 5 seconds                                                                   |
| Wait for a Network Response      | Waits for a specific network response           | await page.waitForResponse(response => response.url() === '<https://example.com/resource>' && response.status() === 200); |
| Wait for a Specific Event        | Waits for a specific event to occur             | await page.waitForEvent('event_name');                                                                                    |

## Script Json File

```Json
{
    "tests":"npx playwright test --project chrome --headed",
    "test":"npx playwright test",
    "chrome":"npx playwright test --project chromium",
    "headed":"npx playwright test --project chrome --headed",
    "report":"npx playwright show-report",
    "ui":"npx playwright test --ui",
    "debug":"npx playwright test --debug",
}
```

## Hooks to run test case

### Only

This will run test case only one time.

```javasccript
test.only('title', async fn)
```

### Skip

This is used to skip test cases from running.

```javasccript
test.skip('title', async fn)
```

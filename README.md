# Codeception Primer
Tutorial taken from https://codeception.com/docs/Introduction

**Codeception** supports all three testing types.
Out of the box you have tools for writing **unit**, **functional**, and **acceptance** tests in a unified framework.
That’s why Codeception consists of three so-called “suites”: A “Unit suite” for all unit tests, a “functional suite” for all functional tests, and an “Acceptance suite” for all acceptance tests.

## 1. Acceptance Tests
https://codeception.com/docs/AcceptanceTests
Run inside a real browser. Have no access to PHP code.

## 2. Functional Tests
Similar to acceptance tests but don't run in a browser.
They are executed
inside PHP without launching a real browser.

## 3. Unit Tests
Test single units of PHP code/classes.
Can also be excuted with Codeception. Codeception offers additional tools and APIs.

## Conclusion
The Codeception framework was developed to actually make testing fun.
It allows writing unit, functional, integration, and acceptance tests in a single, coherent style.
All Codeception tests are written in a descriptive manner. Just by looking at the test body,
you can clearly understand what is being tested and how it is performed.

# Install
New Composer Project with codeception lib:
```
composer require codeception/codeception --dev
```

Run Codeception:
```
php vendor/bin/codecept
```

Init your testing environment with:
```
php vendor/bin/codecept bootstrap
```

# Next Steps
1. Edit tests/acceptance.suite.yml to set url of your application. Change PhpBrowser to WebDriver to enable browser testing
2. Edit tests/functional.suite.yml to enable a framework module. Remove this file if you don't use a framework
3. Create your first acceptance tests using codecept g:cest acceptance First
4. Write first test in tests/acceptance/FirstCest.php
5. Run tests using: codecept run

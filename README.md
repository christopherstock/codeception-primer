# Codeception Primer
Tutorial taken from https://codeception.com/docs/Introduction

**Codeception** supports all three testing types.
Out of the box you have tools for writing **unit**, **functional**, and **acceptance** tests in a unified framework.
That’s why Codeception consists of three so-called “suites”: A “Unit suite” for all unit tests, a “functional suite” for all functional tests, and an “Acceptance suite” for all acceptance tests.

## Acceptance Tests
https://codeception.com/docs/AcceptanceTests
Run inside a real browser. Have no access to PHP code.

## Functional Tests
Similar to acceptance tests but don't run in a browser.
They are executed
inside PHP without launching a real browser.

## Unit Tests
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

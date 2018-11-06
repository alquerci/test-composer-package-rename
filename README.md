Test composer package rename
============================

This is a test package for the purpose of functional testing of packagist behaviour.

Action
------

Update the package name

### Actual

The last commit hash on packagist is frozen on the last commit with the old name.

Action
------

Resubmitting the package to packagist

### Actual

Got a 403 on the webhook (fixed with an update)

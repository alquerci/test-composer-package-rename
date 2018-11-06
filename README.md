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

Action
------

Push new commits and tag

### Actual

On packagist the new package has been auto-updated but not the old one.

Action
------

Mark the old package as "Abandoned" on packagist, and use the new name in the form so that people get pointed to it when they install with the old name.

Trigger manually update on old package.

### Actual

The old package name is still readable. And on next upgrading the deprecation is displayed.

"Package alquerci/test-composer-package-rename is abandoned, you should avoid using it. Use alquerci/test-composer-package-rename-one instead."

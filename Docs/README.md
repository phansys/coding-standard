Doctrine Coding Standard
========================

The Doctrine project follows a coding standard based on
[PSR-2](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md) with custom
additions and modifications.
When contributing to the Doctrine project, the following rules have to be met in order to fulfill this standard.

Control Structures
------------------

- There is no `else if`, you MUST use `elseif` instead.

Formatting
----------

- Corresponding assignment statement tokens MUST be aligned. Assignment tokens are:
  `=`, `&=`, `.=`, `/=`, `-=`, `%=`, `*=`, `+=`, `^=`.
  Each `=` token MUST be on the same column as the one from the previous corresponding statement.

```php
$foo        = 'Foo';
$fooBar     = 'FooBar';
$fooBarBaz  = 'FooBarBaz';
$foo       .= $bar;

$foo = 'Foo';

$object->foo($foo);

$fooBar = 'FooBar';

$object->fooBar($fooBar);

$fooBarBaz = 'FoobarBaz';

$object->fooBarBaz($fooBarBaz);
```

Strings
-------

- The string concatenation token `.` MUST be surrounded by spaces.

## Classes and Namespaces

Namespaces and classes MUST follow [PSR-0](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md).

This means each class is in a file by itself, and is in a namespace of at least one level: a top-level vendor name.

Code written for PHP 5.3 and after MUST use formal namespaces.

Code written for 5.2.x and before SHOULD use the pseudo-namespacing convention of `Vendor_` prefixes on class names.

When present, there MUST be one blank line after the `namespace` declaration and SHOULD be one blank line before it.

When present, all `use` declarations MUST go after the `namespace` declaration.

There MUST be one `use` keyword per declaration.

There MUST be one blank line after the `use` block.

### Extends and Implements

The `extends` and `implements` keywords MUST be declared on the same line as the class name.

Lists of `implements` MAY be split across multiple lines, where each subsequent line is indented once. When doing so, the first item in the list MUST be on the next line, and there MUST be only one interface per line.

### Example

```php
<?php

namespace Vendor\Package;

use FooClass;
use BarClass as Bar;
use OtherVendor\OtherPackage\BazClass;

class ClassName extends ParentClass implements \ArrayAccess
{
    // constants, properties, methods
}

class LongerClassName extends ParentClass implements
    \ArrayAccess,
    \Countable,
    \Serializable
{
    // constants, properties, methods
}

```

### Properties

Visibility MUST be declared on all properties.

The `var` keyword MUST NOT be used to declare a property.

There MUST NOT be more than one property declared per statement.

Property names SHOULD be prefixed with a single underscore to indicate protected or private visibility.
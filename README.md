# Math_Finance

Original repo
https://github.com/pear/Math_Finance

## What Updates are in this fork

* PEAR requirement is removed, all `PEAR::raiseError` is replaced with throwing php `Exception`
* static keyword is added for all static methods
* method visibility keywords are added
* all classes are called from global namespace
* Other small improvements

* PHP 7 compatibility
* Compliance with PSR-0

You should use composer to install it
```
composer require perlitz-group/math_finance
```

After installation add the below code into your composer.json and run `composer dump-autoload`
```
"classmap": [
    "your-vendor-folder/perlitz-group/math_finance/Math",
    "your-vendor-folder/perlitz-group/math_numerical_rootfinding/Math/Numerical"
]        
```

This package is dependent on `Math_Numerical_RootFinding` (requirement is added into composer)
https://github.com/perlitz-group/Math_Numerical_RootFinding


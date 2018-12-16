## Validate Arguments Check

*Note:* Much of this code was taken from another repo. I've lost the link to the original, so I can't reference the original. If you know where this originated please let me know.

### Design by Contract Function

This is used to check that functions and methods are given the correct number of arguments

```php
function myMethod(string $arg1, int $arg2, array $arg3 = null)
{
    assert(check_args());

    // continue with your code
}
```

If `$arg1` or `$arg2` are not supplied you will get an assert error. 
Since the `$arg3` argument is optional it can be left out without error  

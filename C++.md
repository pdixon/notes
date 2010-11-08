# C++

## See Also
[[Qt]]

## References
google coding standard say's reference arguments should always be `const`. i.e:

``` c++
    void foo(const blah &arg);
```
not

``` c++
    void foo(blah &arg);
```
## Initialisers
# C programming language
## This is a collection of various tips and tricks I've acquired on my C programming journey. There is no logic in the ordering of the tips, because I add them as I encounter them.

### IF redundancy
`if (something != 0)` is reduntant, use `if (something)` instead

### for loop doesn't need to have arguments
`for (;;)` is basically the same as `while (true)`

### Tip #3
`exit(0)` is equivalent to `return EXIT_SUCCESS`<br/>
EXIT_FAILURE gives a non-zero value

### Unsigned addition
`   if (ui > UINT_MAX - sum)
    {
        too_big();
    }
    else
    {
      sum = sum + ui;
    }`
### Unsigned subtraction
`
    if (j > i)
    {
        negative();
    }
    else
    {
        i = i - j;
    }`
### Avoid overflow when returning absolute values
`int abs(int i)
{
    return (i >=0) ? i : -(unsigned)i;
}`



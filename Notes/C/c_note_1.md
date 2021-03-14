# C note 1

### __Struct with static__

__Call structure with a function using static.__

``` C
typedef struct s_struct
{
    void *data1;
    void *data2;
}              t_struct;

t_struct *function(void)
{
    static t_struct var = NULL;

    if (!var)
    {
        // malloc var
    }
    return (var);
}
```

__Use like :__

``` C
function()->data1
```

__We can free all data just called function :__

``` C
free(function());
```

### __Cast void *data on other type__

We need cast with (unsigned long). Because sizeof(void *) = 8.  
Example : 

``` C
int main(void)
{
    void *data;
    int i;

    i = 42;
    data = (void *)(unsigned long)i;
}
```
We get a warning if we don't cast with (unsigned long), we can also use (uintptr_t), if we include <stdint.h>.
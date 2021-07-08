# Generalized-List
A short generalized table implementation, you can use this list as you would in python

### example

```c
int main()
{
    // Create List
    //method1
    // ptr_node phead = LIST_(4,
    //     DATA_TYPE,1,
    //     DATA_TYPE,2,
    //     DATA_TYPE,3,
    //     PTR_TYPE,
    //     (LIST_(2,
    //     DATA_TYPE,12,
    //     PTR_TYPE,(LIST_(2,
    //         DATA_TYPE,3,
    //         DATA_TYPE,4))))
    // );
    //method2
    ptr_node phead = CONS(1,CONS(CONS(1,CONS(2,NULL)),CONS(3,CONS(3,NULL))));
    //method3
    CONSTRUCT(ptr_node,obj,2);// auto gc
    // display
    
    displaylist(phead);
    
    //delete
    free_cons(&phead);
    
    
    return 0;
}
```

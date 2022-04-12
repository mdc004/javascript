# metodi utili per

## ordinare randomicamente un array

per ordinare un'array si può modificare il metodo predefinito di ogni array ".sort":

```
  array.sort(function(){
    return Math.random() - 0.5;
  })
```

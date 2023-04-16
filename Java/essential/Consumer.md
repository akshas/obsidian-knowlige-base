## Implement Consumer
```java
import java.util.function.Consumer;

public class MyConsumer<T> implements Consumer<T>{  
  
    @Override  
    public void accept(T t) {  
        System.out.println(t.hashCode());  
    }  
}
```



## Lambda and Link to method as params

```java
    Consumer<String> c1 = a -> System.out.println(String.format("{%s}", a));  
    Consumer<String> c2 = App::linkForCons;  
  
    c1.accept("Hello lambda!");  
    c2.accept("Hello me
    thod!");  
}  
  
public static <T> void linkForCons(T a) {  
    System.out.println(String.format("**** %s ****", a));  
}
```

## andThen
```java
Consumer<String> c1 = a -> System.out.print("*" + a);  
Consumer<String> c2 = a -> System.out.println("*");  
  
var result = c1.andThen(c2);  
result.accept("Hello");
```

## BiConsumer
```java
BiConsumer<String, Integer> biConsumer = (a,b) -> a.repeat(b);  
biConsumer.accept("Hello", 3);


Map<Integer, String> map = Map.of(1, "one", 2, "two", 5, "five");  
map.forEach((a, b) -> System.out.println((b+ " ").repeat(a)));
```

## IntConsumer
``` java
IntConsumer cons = c -> {  
    if(c % 2 == 0)  
        System.out.println("even");  
    else  
        System.out.println("odd");  
};  
  
cons.accept(23); // odd
cons.accept(22); // even
```
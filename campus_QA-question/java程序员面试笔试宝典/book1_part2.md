* example of args[i] input

```java
public class Test {
	public static void main(String[] args){
        for (int i =0; i<args.length; i++){
            System.out.println(args[i]);
        }
    }
}
```

* other main ways

```java
static public void main{
    
}

public static void main{
    
}

public static final void main{
    
}

public static synchronized void main{
    
}

```

* static run first in public method

```java
public Test{
    static {
        Sys.o.p("1");
    }
    p s v main{
        Sys.o.p("2");
    }
    
    // 1
    // 2
}
```


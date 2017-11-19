- java方法重载时怎么在调用方法的时候怎么选取方法？  
  java中允许方法重载，所以我们经常会看到多个名字相同但是参数不同的方法。方法重载后，会有多个方法签名，java编译器会帮我们挑选最符合的那个方法。例：
  ```java
  private void overloadedMethod(Object o) {
    System.out.println("Object");
  }
  private void overloadedMethod(String s) {
    System.out.println("String");
  }
  ```
  调用此方法`overloadedMethod("abc");`会打印`String`。  
  原则是能选子类的就选子类的。如果互相没有子类关系，则编译器报错。
- lambda表达式的类型是什么？  
  lambda表达式的类型就是函数接口的类型。

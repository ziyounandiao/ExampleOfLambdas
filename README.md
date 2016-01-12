# ExampleOfLambdas
lambda 相关demo

1.Examples of lambdas with functional interfaces
use case                             Example of lambda                                 Matching functional interface
boolean Expression               (List<String> list) ->list.isEmpty()                 Predicate<List<String>>
Creating objects                  () -> new Apple(10)                                 Supplier<Apple>
Consuming from an object          (Apple a) -> System.out.println(a.getWeight())      Consumer<Apple>
Select/extract from an object     (String s) -> s.length()                            Function<String, Integer> or ToIntFunction<String>
Combine two values                (int a, int b) -> a * b                             IntBinaryOperator
Compare two objects             (Apple a1, Apple a2) -> 
                                a1.getWeight().compareTo(a2.getWeight())
                                                                                  Comparator<Apple>orBiFunction<Apple, Apple, Integer> 
                                                                                  or ToIntBiFunction<Apple, Apple>

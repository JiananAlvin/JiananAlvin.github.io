---
​---
title: UML
tags: Java 
article_header:
  type: cover

​---

## 
---

# UML

## 1. Class Notation

![image-20230222133043074](https://raw.githubusercontent.com/JiananAlvin/image_bed/master/202302221330216.png)

## 2. Generalization & Realization

```java
public class A extends B { ... }
```

![image-20230222134402596](https://raw.githubusercontent.com/JiananAlvin/image_bed/master/202302221344647.png)

```java
public class A implements B { ... }
```

![image-20230222134329808](https://raw.githubusercontent.com/JiananAlvin/image_bed/master/202302221343856.png)

## 3. Dependency & Association

[[reference]](https://stackoverflow.com/questions/1874049/explanation-of-the-uml-arrows), [[reference2]](https://www.guru99.com/association-aggregation-composition-difference.html)

### 3.0 Cardinality

In UML, cardinality is used to specify the number of instances of one class that can be associated with the instances of another class in an association. 

Here are the different cardinality options and what they mean:

- **1**: Indicates that there can be only one instance of the associated class.
- **0..1**: Indicates that there can be zero or one instance of the associated class. 
- **1..\* or 1..n**: Indicates that there can be one or more instances of the associated class. 
- **0..\* or \* or n..***: Indicates that there can be zero or more instances of the associated class. 
- **m..n**: Indicates that there can be a minimum of `m` instances and a maximum of `n` instances of the associated class. 
- **1..1**: Indicates that there must be exactly one instance of the associated class. This is the same as cardinality of 1.
- **0..0**: Indicates that there can be no instances of the associated class.
- **n..n**: Indicates that there must be exactly `n` instances of the associated class. This is the same as cardinality of `n`.

### 3.1 Dependency

Dependency in UML represents a relationship between two elements where one element, called the **dependent element**, **relies on** the other element, called the **supplier element**, in some way. 

```java
public class Car {
  private Engine engine;

  public Car() {
    engine = new Engine();
  }

  public void start() {
    engine.start();
  }
}

public class Engine {
  public void start() {
    // start the engine
  }
}
```

In this example, the `Car` class depends on the `Engine` class, since it needs an instance of `Engine` to start.
![image-20230222135143787](https://raw.githubusercontent.com/JiananAlvin/image_bed/master/202302221351839.png)

### 3.2 Association

Association in UML represents a relationship between two elements where one element, called the **source element**, **is related to** the other element, called the **target element**, in some way.

#### 3.2.1 Reflexive Association 

```Java
public class Company {
  private Set<Person> employees;
  ....
}

public class Person {
  private Company company;
  ...
}
```

In this example, `Company` has a set of `Person`<span style="color: red">s</span>, and `Person` has a `Company`.

![image-20230222141838403](https://raw.githubusercontent.com/JiananAlvin/image_bed/master/202302221418457.png)

#### 3.2.2 Directed Association

```java
public class Company {
  private Set<Person> employees;
  ....
}

public class Person {
  ...
}
```

In this example, `Company` has a set of `Person`<span style="color: red">s</span>, and `Person` <span style="color: red">does not</span> have a `Company`.

![image-20230222142923697](https://raw.githubusercontent.com/JiananAlvin/image_bed/master/202302221429754.png)

## 4. Aggregation & Composition

please wait for update...



Best,

Jianan
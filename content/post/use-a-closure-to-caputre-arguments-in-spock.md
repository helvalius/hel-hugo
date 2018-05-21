+++
title = "Use a Closure to capture arguments in Spock"
date = 2013-03-26
math = false
highlight = true
draft = false
tags = []
categories = []
preview = false
+++

Just today I have added Groovy tests using [Spock](http://code.google.com/p/spock/) to my maven/tycho build Eclipse plugin. During test migration from [FEST-Assertions](https://github.com/alexruiz/fest-assert-2.x) & [Mockito](http://code.google.com/p/mockito/) I wondered how argument interception in Spock works.

The easy functional solution (that I didn't directly found on the web) is simple: **Use a closure!**

Lets create a simple Person Java class with a name:

``` java
public class Person {
  private String name;

  public void setName(String newName) {
    name = newName;
  }

  public String getName() {
     return name;
  }
}
```

With a Java Test using Mockito one would use an ArgumentCaptor to verify that the name should be John:
``` java
    ArgumentCaptor argument = ArgumentCaptor.forClass(Person.class);
    verify(mock).doSomething(argument.capture());
    assertEquals("John", argument.getValue().getName());
```


So one needs three lines of code to match one expected String. Seems to be quite bloated!

In Spock one can use a Closure to do the same test:
``` groovy
   mock.doSomething({ it.name=="John"})
```
If you want to make sure that you really have a Person, you can also use the explicit Closure:
``` groovy
   mock.doSomething({ Person p -> p.name=="John"})
```

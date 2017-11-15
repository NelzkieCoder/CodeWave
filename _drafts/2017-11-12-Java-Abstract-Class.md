---
layout: post
title: Java Abstract classes
tagline: "A very special kind of class"
image: /assets/patterns/paisley.png
header:
  image: /assets/patterns/asanoha-400px.png
tags: ["Java"]
keywords: Java, OOP, 
lang: en
date: 2017-11-12T08:13:28+00:00
category: articles
---

During my early days of programming, I never knew anything about abstract class. When I finally learned about it, I can't figure out when to use it or am I even gonna use it like ever. I mean why bother using abstract class when I can make a **concret** class make it a base class (other term is 'super class') and derived from it. That change when I get realize that some of the traits of my class share the same trait as my other class. There abstract class started to make sense.

## What is abstract class?
Abstract class is a kind of class that you won't be able to instantiate directly but rather **extend** from it(indirect instantiate).
When I say you can't instantiate it direction, I meant like this
{% highlight java %}
MyAbstractClass myAbstractClass = new MyAbstractClass();
{% endhighlight %}

instead you should indirectly instantiate it like this

{% highlight java %}
public class MyConcreteClass extend AbstractClass{
  // some code here
}
{% endhighlight %}

Although developers prefer interface, **abstract classes** are very important part in Object Oriented Programming(OOP).

## When to use abstract class?

Depending on your design, you can use abstract class when some traits of your class are the same as the other class.

#### **Example**
  Suppose you are a so called "god" and want to create a dog and a cat. Both can eat, sleep, reproduce. These are traits that are needed for survival. If we won't be using abstract class our code will look like this

  
{% highlight java %}
public class Dog {

    private void CanEat(){
        System.out.println("Dog can eat");
    }
    private void CanSleep(){
        System.out.println("Dog can sleep");
    }
    private void CanReproduce(){
        System.out.println("Dog can reproduce");
    }
}


public class Cat {
  
    private void CanEat(){
        System.out.println("Cat can eat");
    }
    private void CanSleep(){
        System.out.println("Cat can sleep");
    }
    private void CanReproduce(){
        System.out.println("Cat can reproduce");
    }
}

{% endhighlight %}

Looks easy right? Now since you are a "god" you get excited and wanted to create more animals. So you created a lot of animals till your heart's content. But then all of a sudden, you got bored because you are just only copy pasting code from other class to the new class. Boring! Now, can you see the problem here? All of the animals created share the same survival trait. So you think of something to lessen your work. You figured out that these cats and dogs, are both **animals**, so instead of puting the same code on all of the classes, you put it on concrete **animal class** and then derived from it. Your code will now look like this


{% highlight java %}

public class Animal {

    public String name = "Dog";

    protected void CanEat(){
        System.out.println( name + " can eat");
    }
    protected void CanSleep(){
        System.out.println(name + " can sleep");
    }
    protected void CanReproduce(){
        System.out.println(name + " can reproduce");
    }
}

public class Cat extends Animal {
    public Cat() {
        this.name = "Cat";
    }
}

public class Dog extends Animal {
    public Dog() {
        this.name = "Dog";
    }
}


public static void main(String[] args) {

        Dog dog = new Dog();
        dog.CanEat();
        dog.CanSleep();
        dog.CanReproduce();


        Cat cat = new Cat();
        cat.CanEat();
        cat.CanSleep();
        cat.CanReproduce();
    }

{% endhighlight %}
{% highlight java %}
Output:
Dog can eat
Dog can sleep
Dog can reproduce
Cat can eat
Cat can sleep
Cat can reproduce

{% endhighlight %}

That is a huge improvement. You can now create as much animals as you want with minimal changes of your code. Awesome! Now you get tired and decided to sleep. Unfortunately one of your angels saw what you're doing and decided to mess with things. 

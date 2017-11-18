---
layout: post
title: Java Fundamentals 101
tagline: "Variables and Data types"
image: /assets/patterns/paisley.png
header:
  image: /assets/patterns/asanoha-400px.png
tags: ["Java"]
keywords: Java, Fundamentals, Basic, Arrays
ref: post-example-in-english
lang: en
date: 2017-10-28T08:13:28+00:00
category: articles
---

## **Fundamentals. First things first**

Keep in mind that fundamentals don’t just apply to single programming language. In fact, it applies to any other programming language out there. Just like when you learn how to drive, it doesn’t apply only to a car made by Toyota, you can also drive ford or audi or Tesla. In this tutorial, I am using Java. There might be a small syntax change when using different language but the logic remains the same.

<!--break-->

## What Is Fundamentals and why is it so important?

Base on google search it means **"a central or primary rule or principle on which something is based"**. Think of it this way, every complicated shape that you can draw start with a simple one(it can be square or circle or triangle).  If you want to be a good artist, you have to know when to use this shapes and how it correlates to the other shape. It's all the same for programming. If you want to be a good programmer, you have to understand the fundamentals of programming. Do you want to be a good programmer? If so, then lets proceed.

<!--more-->

### Topics:

  * Variables
  * Data Types

### **Prerequisites**

[JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html), [Intellij Idea Community Edition](https://www.jetbrains.com/idea/) or [Eclipse IDE](https://www.eclipse.org/ide/)(_Though I recommend Intellij, Eclipse is just a pain to work with_). Install it. I am not gonna show you have to do that. Cmon, you know how to browse the web, I am pretty sure you know how to install stuff on your computer. If you don’t know how to install, I suggest googling it.


### **Target Audience**

People with no programming experience and just want to know and gain deeper knowledge of the basics.

### **Creating a Java File**

  * Create new Project

<img class="alignnone size-medium wp-image-171" src="http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-10.22.28-PM-300x285.png" alt="" width="300" height="285" srcset="http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-10.22.28-PM-300x285.png 300w, http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-10.22.28-PM.png 476w" sizes="(max-width: 300px) 100vw, 300px" />

&nbsp;

  * Click Next until you are on the Project name box.
  * Name your Project &#8220;**LessonOne**&#8220;
  * Select the src folder. **Right click** then select **New**.
  * Select **Java Class**
  * Name it **Main**

<img class="alignnone size-medium wp-image-167" src="http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-9.59.13-PM-300x63.png" alt="" width="300" height="63" srcset="http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-9.59.13-PM-300x63.png 300w, http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-9.59.13-PM.png 525w" sizes="(max-width: 300px) 100vw, 300px" />

Inside the main class type

{% highlight java %}public static void main(String[] args) {
    
}{% endhighlight %}

<img class="alignnone wp-image-169 size-medium" src="http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-10.02.18-PM-300x80.png" alt="" width="300" height="80" srcset="http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-10.02.18-PM-300x80.png 300w, http://nelzkiea.sgedu.site/nelzkie_coder/wp-content/uploads/2017/10/Screen-Shot-2017-10-28-at-10.02.18-PM.png 690w" sizes="(max-width: 300px) 100vw, 300px" />

Now. You&#8217;re done.

### **Let&#8217;s get started**

#### **Variables**

What are variables? Variables sort of act like a piece of data that we can use or manipulate depending on our needs. It looks something like this

{% highlight java %}int mynumber = 1; {% endhighlight %}

A **variable** is composed of 3 parts. The data type in the example its the &#8220;**int**&#8220;, the variable name here its&#8217; **&#8220;mynumber&#8221;,** and the value which is **1**.



#### **Data Types**

##### **There are 2 types of Data tpes**

  * The **primitive** data types
  * The **object** data types

For now, we will focus on primitive data types. I don’t want to overwhelm you with advance topic.

**Primitive Data Type**

There are 8 primitive data types.

  * Boolean
  * Byte
  * Char
  * Short
  * Integer or int for short
  * Long
  * Float
  * Double



#### **Boolean**

  * A Boolean consist of true or false. 1 or 0.
  * Default value is false {% highlight java %}boolean letmeguess = true;  {% endhighlight %}

#### **Integer**

  * An integer is usually used when you have a numerical value that is not decimal
  * The maximum value you can have in an int is **2,147,483,647.** The minimum is **-2,147,483,647**
  * Default value is 0
  * Consist of 4 bytes {% highlight java %}int mynumber = 125000;  {% endhighlight %}

#### **Long**

  * Long is like Integer but with greater value
  * Maximum value is **9,223,372,036,854,775,807**
  * Minimum value is **-9,223,372,036,854,775,807**
  * Default value is 0L
  * Consist of 8 bytes {% highlight java %}int mylong = 10000000L;  {% endhighlight %}

#### **Short**

  * Short is an integer but is smaller than Integer data type
  * Minimum value is -32,768
  * Maximum value is 32,767
  * Consist of 2 bytes {% highlight java %}int myShort = 2000;  {% endhighlight %}

#### **Float**

  * Float is use rarely other than when you’re doing a game as you need to use it in some advance calculation
  * Default value is 0.0f
  * Consist of 4 bytes
  * 6-7 decimal digits’ precision {% highlight java %}int myFloat = 10.9f; {% endhighlight %}

#### **Double**

  * A Double is like a float but has a greater range of decimal numbers
  * 15-16 decimal digits
  * Default value is 0.0d
  * Consist of 8 bytes {% highlight java %}int myDouble = 102.905d;  {% endhighlight %}

#### **Byte**

  * Byte is the smallest of all primitive types. 4 times smaller than an Integer. It only consists of 8 bits or 1 byte
  * Maximum value is 127
  * Minimum value is -128
  * Default is 0 {% highlight java %}byte b = 1; {% endhighlight %}


#### **Char**

  * A char is a 16 bits Unicode character (E.g &#8216;a&#8217;, &#8216;\u0041&#8217;, &#8216;\101&#8217;, &#8216;\\&#8217;, &#8216;\&#8221;, &#8216;\n&#8217;, &#8216;ß&#8217;)
  * In normal terms, a char is a letter
  * Minimum value is &#8216;\u0000&#8217;
  * Maximum value is &#8216;\uffff&#8217; {% highlight java %}char a = 'a'; {% endhighlight %}


&nbsp;

#### **Woah woah woah! Where is the String man?**

If you declare a variable with String data type. That means string is an object data type. Why? Because String is an object. To be precise an array of chars. Think of string as something like this

{% highlight java %}char[] string = {'h','e','l','l','o'};
{% endhighlight %}

we have not discussed arrays yet. We will discussed it  later on the next topic, for now ignore it.

&nbsp;

### How do we used these variables in a program?

There will be a bit of advanced topic that we haven&#8217;t covered yet so please don&#8217;t let it bother you and just ignore it for now.

Here is the code

{% highlight java %}
public static void main(String[] args) {
    char a = 'a';
    int x = 100000;
    float f = 10f; // or 10.0f
    double d = 100.013d;
    long l = 100000000L;
    byte b = 1;
    short s = 2000;
    boolean bool = true;
    char[] stringmadeofchars = {'h','e','l','l','o'};

    System.out.println("The char is " + a);
    System.out.println("The int is " + x);
    System.out.println("The float is " + f);
    System.out.println("The double is " + d);
    System.out.println("The long is " + l);
    System.out.println("The byte is " + b);
    System.out.println("The short is " + s);
    System.out.println("The boolean is " + bool);

    String helloString = new String(stringmadeofchars);
    System.out.println("Our string is " + helloString);
}{% endhighlight %}

&nbsp;

The {% highlight java %}System.out.println(){% endhighlight %}

is a function that displays the data inside of the parenthesis in the console window of Intellij Idea.

Notice the **new** keyword and the **+** sign there? Yeah the **new **keyword is use when declaring an object which well cover when we get to classes and objects and the **+** sign is what we call an &#8220;**operator**&#8221; which we&#8217;ll cover on the next topic. For now try the code on your own and be amazed!

Congratulations, you have now created a simple program. You can download the full source code **[here](https://github.com/NelzkieCoder/CodeWithEase/tree/master)**

You are now officially a programmer. A beginner programmer that is. But hey, remember that every **PRO** was once a **BEGINNER.**

On the next topic we&#8217;ll  cover arrays.

&nbsp;
---
layout: post
title: "Java Arrays"
tagline: "Learning how to use arrays"
image: /assets/patterns/paisley.png
header:
  image: /assets/patterns/asanoha-400px.png
date: 2017-10-28T08:13:28+00:00

tags: ["Java"]
keywords: Java, Fundamentals, Basic, Arrays
ref: example-project-page
lang: en
category: articles
---

### Arrays
What is an array? Think of array as a collection of data or information. It can be a collection [primitive type][jekyll-docs] we discuss earlier or objects(like classes) which we'll discuss on future topic.




<!--break-->

#### Array types
##### **Primitive type array**

To initialize a primitive type array with no defined max size limit, we initialize it like this:

{% highlight java %}
int[] intArray = {1,2,3,4,5,6,7,8}; // you add as many element as you want
char[] chars = {'a','b','c','d'};
{% endhighlight %}

we could also declare the max size of the array which is this example the max is **5**
{% highlight java %}
int[] intArray4 = new int[5]; // default value of all 5 element is 0
{% endhighlight %}

##### **Object type array**
To initialize an object array with no defined max size limit, we initialize it like this:
{% highlight java %}
  String[] strings = {"Hello","World","Code","and","Wave"}; // this is an object 
  MyClass[] myClasses = {new MyClass(),new MyClass()};  // this is an object too
{% endhighlight %}


<br/>
<p><span class="warning"> <span style="font-weight:bold;">NOTE:</span> Keep in mind that strings are objects and not primitive type</span></p><br/>
We haven't covered objects and classes yet so as always just skip that part for now. I Just put it there to state that **arrays** can be primitive and non-primitive.

#### Displaying specific element of an array?
This can be a bit confusing. Say for example we have an array of int like this
{% highlight java %}
int[] intArrays = new int[5];
intArrays[0]=10; // On index 0 we assign value of 10
intArrays[1]=20; // On index 1 we assign value of 20
intArrays[2]=30; // On index 2 we assign value of 30
intArrays[3]=40; // On index 3 we assign value of 40
intArrays[4]=50; // On index 4 we assign value of 50

 System.out.println(intArray4[0]); // will display 10
{% endhighlight %}

on the example the **intArrays[0]** is the first element which we assign a value of 10. Then what is **index**? Index is the position of a certain element inside of the array. To visualize it. Take a loot at this image

![My helpful screenshot]({{ "/assets/image/arrays.png" | absolute_url }})

The <span style="color:blue"> **blue** </span> ones are the value we assign and the <span style="color:red"> **red** </span> ones are the **indexes**(or indices????) so when we display an element of array we do it like this:
{% highlight java %}
int[] intArrays = new int[5];
System.out.println(intArray4[0]); // will display 10
{% endhighlight %}

although we haven't covered loop yet, we could also loop through the whole array and display each element
{% highlight java %}
int[] intArrays = new int[5];
for (int a: intArrays){
  System.out.println(a); // will display each element
}

{% endhighlight %}


Here is the whole code
{% highlight java %}
public static void main(String[] args) {


        int[] intArray = {1,2,3,4,5,6,7,8};
        char[] chars = {'a','b','c','d'};

        int[] intArrays = new int[5];
        intArrays[0]=10;
        intArrays[1]=20;
        intArrays[2]=70;
        intArrays[3]=40;
        intArrays[4]=50;
        System.out.println(intArrays[0]);

        String[] strings = {"Hello","World","Code","and","Wave"};
        
        for (int a: intArrays){
            System.out.println(a);
        }
        
    }
{% endhighlight %}


Instead of declaring a lot of variable with the same [data type][jekyll-docs], we could instead use an array and just call the element by index. Hopefully you now have a better understand of how array works. 

[jekyll-docs]: {{ site.baseurl }}{% post_url 2017-10-28-152-Java-Fundaments-1 %}
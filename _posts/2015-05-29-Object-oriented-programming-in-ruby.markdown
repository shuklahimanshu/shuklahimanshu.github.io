---
layout: post
title:  "Object oriented programming in Ruby"
date:   2015-05-29 10:53:00
categories: jekyll update
---
<h1> Ruby and Oops </h1>
<p align = "justify">
Object oriented programming serves as a powerful tool in the programming
world. It relates the program to the real world like problems. Although
everything in Ruby is an object, defining your own objects of
requirement makes the work much more easy and organized.
This is achieved by making classes. A class is like a factory that
produces kind of objects that we need. It helps in division of program
into sections with defined functionality. For example, if you want to
write a program to calculate distance between two points, you can make a
class named Point (it is conventional to CamelCase class names in Ruby).
Two objects of this class will represent two different points in
coordinate space (or they may be same). Defining classes is always
helpful if you want to write a large code. But there can be cases when
making a class is meaningless. You should just ask these questions to
yourself :

<ul>  
<li>"What an object of this class would represent and how any two objects
of the class would be different ?"</li>
<li>"What would be the properties (or attributes) of this class ?"</li>
<li>"What functionalities or methods would this class need (if any)
  ?"</li>
</ul>  
</p>

<p align = "justify">  
To make the code more organized, each class should be written in a
different file and name of the file should be same as that of the class.
This makes the code more readable, easy to follow when there are
multiple contributors and last but not the least, simple.
</p>
<p align = "justify">
First thing after defining a class is to write its initialization
method, also known as constructor. This method, when invoked, assigns
values to the class attribues. After this comes the answer to the third and final question - methods
of the class. You don't need to know all the methods that the class
should contain before starting with the methods. In fact, you almost
never know all of them. They come to you as your code grows and as your
needs and expectations with the code increase. This is what oops equips you with - an easy way to expand
your code. Adding methods, as per need, is the best way to expand the
code and add more and more functionalities to the program. But one thing
should always be kept in mind while writing a method - the method should
not go out of class' context. For example, if you have another class
Line, in addition to Point, with attributes start_point and end_point,
then in order to find out common point between two lines, the method
should be inside Line class and not Point class. Also, in order to find
the common point, you will need to compare the points. Method for equality of
points should be contained inside Point class. The context also depends
on how you define your method; for example, calculating the length of a
line is same as finding the distance between two points. So if you
define a method length(), it should be contained inside Line, and if you
choose distance_between() as your method, it should be a part of Point
class. In this particular case, an in between solution exists -
distance_between() can be defined in Point and length() can call
distance_between() and return the result. This will allow the program to
be more easy to use and handle.
</p>
<p align = "justify">
Oops is all about making the code more organized, more easy to
understand, more easy to expand and better in every other sense. There
is another great concept that every programmer who wants to implement
oops, should know. It is called S.O.L.I.D. (abbreviated for five important
programming principles) - 
<ul>
<li>S – Single-responsiblity principle</li>
<li>O – Open-closed principle</li>
<li>L – Liskov substitution principle</li>
<li>I – Interface segregation principle</li>
<li>D – Dependency Inversion Principle</li>
</ul>
A nice blog is written on S.O.L.I.D. - https://scotch.io/bar-talk/s-o-l-i-d-the-first-five-principles-of-object-oriented-design.
</p>

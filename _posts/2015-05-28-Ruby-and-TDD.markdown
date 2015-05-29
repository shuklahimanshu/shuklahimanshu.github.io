---
layout: post
title:  "Ruby and Test Driven Development"
date:   2015-05-28 19:18:58
categories: jekyll update
---
<h1> Ruby and Test Driven Development </h1>


Ruby is an object oriented programming language. It tries to implement this idea everywhere with the simple philosophy of “everything is an object.” Syntaxes of ruby are much more like english language and this makes them quite intuitive. You can sometimes write an unknown syntax just based on your intuition. Ruby also allows method calls in a chain, like object.method_1( ).method_2( ).method_3( ) and so on.  This way of writing codes in ruby crunches the code to quite a smaller size. Also, there are several ways of doing the same thing ruby.

Ruby conventions – It is conventional in ruby to name a method in small cases with underscores, called as snake casing. A class is named in camel casing. Also, methods that return boolean values are named with a question mark at the end – method_to_return_boolean?

Ruby has a vast collection of libraries called gems.

Namespacing is a way of bundling logically related objects together. Modules serve as a convenient tool for this. This allows classes or modules with conflicting names to co-exist while avoiding collisions.

Test driven devenlopment (TDD) is a better way of wrting codes. Here, the objectives are defined first and are put in the form of tests. After writing the tests, code is written and tested to pass. If it fails, then the logic is modified, but the tests remain intact. This results in reduction in scope of errors and makes debugging quite easy. Even if a different person starts working on the code and changes it entirely, the output remains intact. So, for a package with a large number of files and each contains file thousands of lines of code, modification in code with TDD, reduces the chances of error by a much greater extent.

Testing is also of different types – integration testing and unit testing. In Unit testing, code is divided in units and each unit is tested separately. While in integration testing, only the final outcome of the whole program matters. Functioning of individual units is not taken into account.

Several gems are available that make the testing easy. Rspec is one of them.

Conventions in programming are followed so that different contributors can understand each other’s work easily. One of the convention is to structure the code into two directories named lib and spec (test in general. Spec is created because of rspec). Bundler is a dependency management package for ruby. It creates a Gemfile that lists down the gems required by the program being written. This helps when different authors work on same code and saves from different versions of same gem on different machines.

Git is a distributed version management system. It allows programmers to keep track of changes in the program. Github is a public repository where people share their codes and anyone can contribute in the program.

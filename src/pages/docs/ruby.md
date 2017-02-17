---
title: "Ruby"
description: "Learn about Ruby"
layout: "guide"
icon: "code-file"
weight: 4
---

#### References
* [Ruby tutorial](https://www.codecademy.com/learn/ruby)
* [Ruby docs/tutorial](http://www.tutorialspoint.com/ruby)
* [RegEx learning tool](http://regexr.com)
* [CSS selector reference](http://www.w3schools.com/cssref/css_selectors.asp)

<article id="article1">

## Goals

1. Get to know basic Ruby syntax.
1. Be able to write code using conditional logic and loops.
 	* Know how to to loop through contents of a cucumber table.
1. Understand basic object oriented concepts (i.e. classes, inheritance, etc. )
1. Understand basic page object design.
 	* What are the advantages of using page objects?

</article>

<article id="article2">

## Reading

[Page object pattern](http://blog.josephwilk.net/cucumber/page-object-pattern.html)

[Acceptance tests with page objects](https://robots.thoughtbot.com/better-acceptance-tests-with-page-objects)

</article>

<article id="article3">

## Exercises

Write the scenarios and step definitions for Exercises 1 and 2.

#### Exercise 1

1. Sign in to https://www-support-2.liferay.com/group/customer
2. Navigate to LESA Search page
3. Do a keyword search for "QAPROJECT1"
4. Assert that 1 or more result rows are displayed
5. Print to console the number of tickets found

#### Exercise 2

Same as above, except steps 3 to 5 will be repeated for multiple projects:

Use a cucumber table in the feature file and use the table methods to loop through each of those projects.
* QAPROJECT1
* QAPROJECT2
* THESPACEPRO

#### Exercise 3

Create a page object for the LESA Search page.  Include "element locator" and "action" methods you need from the previous exercise.  Refactor the step definitions from the previous exercise to use the page object.

### Bonus
Can you figure out how to use cucumber tags to run a single scenario?

</article>

---
title: "Cucumber"
description: "Learn about Cucumber"
layout: "guide"
icon: "flash"
weight: 2
---

#### References
[Cucumber wiki](https://github.com/cucumber/cucumber/wiki)

<article id="article1">

## Goals

1. Explore BDD (Behavior Driven Development) concepts
 	* What is it?
 	* What are some benefits of using BDD?
1. Understand these components of a cucumber test:
	 * Feature
	 * Scenario
	 * Step
	 * Step Definition
1.  Be able to run a cucumber test.

</article>

<article id="article2">

## Reading

[Cucumber introduction](https://blog.engineyard.com/2009/cucumber-introduction)

[Why use BDD?](http://www.agile-doctor.com/2012/03/06/10-reasons-why-bdd-changes-everything/)

[Feature](https://github.com/cucumber/cucumber/wiki/Feature-Introduction)

[Gherkin](https://github.com/cucumber/cucumber/wiki/Gherkin)

[Given-When-Then](https://github.com/cucumber/cucumber/wiki/Given-When-Then-%28new%29)

[Step Definitions](https://github.com/cucumber/cucumber/wiki/Step-Definitions)

</article>

<article id="article3">

## Exercises

In the following exercises, you will be writing the test steps in the .feature file.  At this stage, you are not writing the step definitions.

To begin:
* Create a 'cucumber-practice' folder.
* Go to the command line and run `cucumber --init` from this directory.  Examine the default folder structure and files that were created.
* Create a file called 'practice.feature' in the feature directory.

Write these scenarios in practice.feature.  Each scenario should contain at least one of each [Given-When-Then].

1. Write a scenario that signs the test user in to LESA.  (Your trainer will show you the manual steps for doing this.)

2. Write a scenario that does a google search for 'Liferay', then navigates to Liferay home page by clicking on the correct search result.

Run the cucumber scenarios:
* Add the following to env.rb (in cucumber-practice/features/support)

```ruby
require 'selenium-webdriver'
require 'rubygems'
require 'capybara'
require 'capybara/cucumber'

Capybara.register_driver :selenium do |app|
  	Capybara::Selenium::Driver.new(app, :browser => :chrome)
end

Capybara.default_driver = :selenium
```

* At the command line, run `cucumber features`.
* What output do you see in the terminal?

</article>

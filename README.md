# AndroidTestingBox

Android project to experiment various testing tools.
It targets **Java** and **Kotlin** languages.
Priority is given to fluency and ease of use.
The idea is to provide a toolbox to write elegant and intelligible tests, with modern techniques like **behavior-driven testing frameworks** or **fluent assertions**.

[![Dependency Status](https://www.versioneye.com/user/projects/58261d9e7a72950483fd3428/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/58261d9e7a72950483fd3428)
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-AndroidTestingBox-brightgreen.svg?style=flat)]()

## JUnit

### Frutilla

- https://github.com/ignaciotcrespo/frutilla

### Fluent test method names

- https://jijeshmohan.wordpress.com/2011/12/17/junit-readable-test-names/

### Fluent assertions: truth

- https://google.github.io/truth/

#### Alternative: AssertJ (http://joel-costigliola.github.io/assertj/)

### Specifications framework: Spectrum

- https://github.com/greghaskins/spectrum
- http://www.greghaskins.com/archive/introducing-spectrum-bdd-style-test-runner-for-java-junit

#### Alternative: Oleaster (https://github.com/mscharhag/oleaster)

### Hierarchies in JUnit: junit-hierarchicalcontextrunner

- https://github.com/bechte/junit-hierarchicalcontextrunner

### BDD tool: JGiven

- http://jgiven.org/

### Mutation testing: Zester plugin

- https://plugins.jetbrains.com/plugin/8281
- https://tech.zalando.com/blog/zester-mutation-testing/

For this sample project, define a new "Run configuration" with Zester such as:

```
Target classes: com.guddy.android_testing_box.zester.*
Test class: com.guddy.android_testing_box.zester.ZesterExampleTest
```

It generates an HTML report in the `build/reports/zester/` directory, showing that 2 "mutants" survived to unit tests (so potential bugs, and in this case, yes it is).

## Kotlin 

### Specifications framework: Spek

- https://github.com/JetBrains/spek
- http://jetbrains.github.io/spek/docs/latest/#setting-up

### Fluent assertions: Kluent

- https://github.com/MarkusAmshove/Kluent

#### Alternative: Expekt (https://github.com/winterbe/expekt)

### Alternative to JUnit: TestNG (http://testng.org/doc/index.html)

## Android

### Fluent assertions: AssertJ Android

- http://square.github.io/assertj-android/

### Robotium

- https://github.com/RobotiumTech/robotium

## IDE configuration

- MoreUnit plugin:  https://plugins.jetbrains.com/plugin/7105

# Nota Bene

A relevant combination of [Dagger2](https://google.github.io/dagger/) and [mockito](http://site.mockito.org/) is already described in a previous post I wrote: http://roroche.github.io/AndroidStarter/

# Bibliography

- https://blog.codecentric.de/en/2016/01/writing-better-tests-junit/
- https://www.petrikainulainen.net/programming/unit-testing/3-reasons-why-we-should-not-use-inheritance-in-our-tests/
- http://blog.xebia.com/mutation-testing-how-good-are-your-unit-tests/

# Interesting repositories

- https://github.com/googlesamples/android-testing
- https://github.com/TNG/JGiven/tree/master/jgiven-examples
- https://github.com/ahus1/bdd-examples

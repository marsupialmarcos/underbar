#### underbar
This is a project I completed as a student at [hackreactor](http://hackreactor.com). This project was worked on with a pair.

# UNDERBAR REVIEW

This project was written in the same spirit as JavaScript Koans, and thusly uses the Mocha Test Suite to facilitate a TDD approach to learning. It walks you through a reimplementation of underscore.js, a popular collection of useful functions authored by Jeremy Ashkenas.

#  REVIEW SPRINT REPO
The repo you will be working out of will be a different repo from Precourse. Look on Github for underbar-review instead of underbar. Work on this from scratch and do not reference code from Precourse.

# POMANDER
To ensure your work is of the highest quality, we've created Pomander, a tool that checks your code for syntax errors and violations against the style guide before each commit.

Install it by navigating to this repository in Terminal and running the following command:
 
```javascript
curl -s https://raw.githubusercontent.com/reactorcore/pomander/master/bin/install | bash
```

Pomander uses a pre-commit hook to run staged files through eslint before each commit. eslint is a linter that will block your commit should you have any syntax errors, or, should you violate the Hack Reactor style guide. There are some preferred whitespace style rules that will give warnings but not block your commit. If the linter gives you any funny bugs, these bugs are not intentional, and you should feel free to skip using it during commits with the --no-verify option.

# BROKEN TESTS
To help you familiarize yourself with our favorite testing tools, Mocha and Chai, we've broken the test suite.

Mocha is a test framework that provides the structure for test files, and is responsible for running tests and reporting their results. Mocha provides the it and describe global variables along with useful hooks like beforeEach.

Chai is an assertion library that makes your tests more expressive and your error messages more helpful. Chai provides the expect function and various methods that allow you to express your behavior in a human readable way.

Pay careful attention to the test files and fix them as necessary. Do not to refer back to the previous test suite, you would only be cheating yourself out of an important learning opportunity. Instead, use the Mocha and Chai documentation. You can do it!

NO MORE NOTES

For your convenience, the "Links and Resources" section has been removed. As you continue your journey as a developer, one of the most valuable skills you can build is the ability to efficiently look up what you don't understand. Practice this skill every chance you get.

# BARE MINIMUM REQUIREMENTS
As is, the repository is missing code for most of the functions. It's your job to fix the library by implementing them. The functions are split in two sections, with a separate test suite for each.

The files in the spec directory contain the test suites. Your goal is to fix any tests that are broken and then get them all to pass by implementing the missing functions. Run all the tests by opening SpecRunner.html in your browser.

The file src/underbar.js contains function definitions and explanations for the following functions (italicized functions are solved for you but contain broken tests). Implement each of the functions:

# PART I:
identity

first

last

each

indexOf

filter

reject

uniq

map

pluck

reduce

# PART II:
contains

every

some

extend

defaults

once

memoize

delay

shuffle

Note: JavaScript provides some built-in Array functions--including forEach, map, reduce and filter--that replicate the functionality of some of the functions you will implement. Don't use them to implement your functions.

# ADVANCED CONTENT
Ensure the tests for all previously solved functions (italicized above) are fixed
Use checkForNativeMethods to write a test for each function that will fail if a built-in Array function is used

Implement the following functions:

invoke

sortBy

zip

flatten

intersection

difference

throttle

There's one function that is a little more complicated, so we've included some more context to help you along.

```javascript
_.throttle(func, wait): Wrap a function func so that it can be called at most once within a period of wait milliseconds. This is useful for throttling access to expensive APIs or to drawing routines in a video game. Let's see how it's used:

var counter = 0;
var increment = function() {
  return counter += 1;
};

// Create a function called throttledIncrement. This function can be called at
// most once every 100ms
var throttledIncrement = _.throttle(increment, 100);

throttledIncrement(); // return 1; `counter` should now be 1

Arguments passed to the throttled function should be passed to the original function. The throttled function should always return the most recently returned value of the original function. If the wait period is 100ms and the function was last called 30ms ago, another call to the throttled function should schedule a call for 0ms after the wait period is over.
```

# NIGHTMARE MODE

The ECMAScript specification is a scripting language specification upon which JavaScript implementations (such as those found in web browsers like Chrome) are based. In June 2015, the 6th edition of the ECMAScript standard was finalized, and is commonly referred to as ES6.

ES6 introduces a wealth of new features to JavaScript while being entirely reverse-compatible with older JavaScript. Even the most popular of web browsers like Chrome have a ton of work to do before all ES6 features are available, however, a lot of developers are using ES6 features and you should look forward to seeing more and more of ES6 in the next several years.

You can play around with ES6 in the latest version of Chrome.

Visit chrome://help in Chrome and ensure that you are using version 49 or above. Once you're up to date with the latest version, Chrome will accept and run many new ES6 features, allowing you to attempt the refactor described next.

Refactor with ES6 Arrow Functions and Rest parameters

ES6 introduces a slick new feature called arrow function expressions that provide syntactic sugar to make anonymous higher order functions (such as those you have been building out during this Underbar sprint) much more concise. Arrow function expressions also provide lexical scoping to the this value.

ES6 also provides a feature called rest parameters which provide syntactic sugar for making your work with function parameters much more appealing.

Refactor your already-test-passing Underbar functions to helpfully utilize arrow function expressions and rest parameters. Assuming your refactors are correct, and that you have enabled experimental JavaScript in the step above, your tests will continue to pass

MDN is the source of truth for JavaScript. Refer to MDN's arrow function expression and rest parameter documentation for reference and helpful information to get started.

Important Note: Again, our advanced content is intended to throw you in over your head. It is expected you feel underprepared for this particular task. Be strong and enjoy moving into the unknown. You will thrive in this industry if you learn to love learning with little support. Go make some mistakes, collaborate with your team, and figure it out. You got this!

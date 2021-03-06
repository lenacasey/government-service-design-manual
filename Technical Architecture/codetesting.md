#Testing code
We use automated testing to ensure that our code does what is intended, to protect against mis-use of that code, and to provide assurance that iterating that code for better design or new features doesn't break existing behaviour. We also add manual testing as an extra check where appropriate.

##Guidance/Tool
Any code written for your service should have a suite of tests operating at two levels:
* "acceptance testing" requires broad tests that run through high-level functionality end-to-end making sure that the pieces of the system come together to provide the right service. A developer should be able to describe the steps in any acceptance test to the product/service owner in a way that makes sense to them and matches how they expect the service to be used (or abused!)
* "unit testing" is focussed on the specific details of the code ensuring that each discrete unit of code does what is expected of it. They allow the developers to verify that complex calculations are performed correctly, to ensure that code handles bad input properly, and that optimisations to the code don't break its behaviour.

We aim to write a first set of tests at the start of working on a feature. An acceptance test that describes the end-to-end behaviour ensures that everyone involved understands the objective of a piece of work, and can demonstrate progress through the story at hand. Unit tests can then be written to understand the implementation of the code.

Tests are often described as "happy path" or "sad path". Happy path tests verify that the system can be used as intended, while sad-path tests verify that it handles errors (whether bad input from a user, a vital API being unavailable, or some other issue) gracefully. We start with happy path tests and a few simple sad path tests and then add more sad path tests as our understanding of the code and its dependencies develops.

Tests should also be written whenever a bug is discovered. A test to reproduce the bug should be written before it is fixed, allowing you to verify that the bug has been fixed and ensure that it isn't reintroduced later.

Developers are expected to run tests regularly, especially before sharing new code, they are verified as part of the code review process, and they are also run regularly in a shared continuous integration system to ensure the whole team has a chance to see how they're performing.

##Code/Templates
If you're giving people code r copy to cuta and paste then here is where it will go.

##Why we do this
This is the reasoning for the decision. You might want to link to relevant blog posts or legislation here.

##Further reading
Link within the Manual, or to other posts, that will help people to work on the tool.
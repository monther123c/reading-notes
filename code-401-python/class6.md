# oop 2
---
# What are Design Patterns
Software design patterns are reusable solutions to common problems in software development. As the name suggests, however, a software design pattern is not code – rather, software design patterns act as a guide or paradigm to help software engineers create products following best practices.
-In the case of object-oriented programming paradigm, design patterns are generally aimed at solving the problems of object generation and communication, rather than the larger scale problems of overall software architecture.
---
# Risk Analysis
Risk analysis is the process of identifying and analyzing potential issues that could negatively impact key business initiatives or projects. This process is done in order to help organizations avoid or mitigate those risks.

Risk Analysis allows you to examine the risks that you or your organization face, and helps you decide whether or not to move forward with a decision.

Risk Identification :

There are different sets of risks included in the risk identification process. Those are as follows:

Business Risks : any exposure a company or organization has to factor(s) that may lower its profits or cause it to go bankrupt.

Testing Risks

Premature Release Risk : a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

Software Risks : probability of occurrence for uncertain events and their potential for loss within an organization.

Risk Assessment : is the process of identifying what hazards currently exist or may appear in the workplace.

The perspective of Risk Assessment

Effect : To evaluate risk based on the effect. If you identify a condition, event, or action and try to assess its significance.

Cause : Assessing risk by Cause is the inverse of assessing risk by Effect. Begin scanning the problem and working your way to the point where you believe the most likely cause is.

Likelihood : To assess risk using Likelihood means to say that there is a chance that a requirement will not be met.

How to Conduct a Risk Analysis

There are three steps to take:

Looking for the danger

Examining the consequences of each individual risk

Risk mitigation strategies
---
# Dependency Injection
dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object.
A dependency is an object that can be used (a service).

When class A uses some functionality of class B, then its said that class A has a dependency of class B.

Three types of dependency injection:
1, constructor injection: the dependencies are provided through a class constructor.
2, setter injection: the client exposes a setter method that the injector uses to inject the dependency.
3, interface injection: the dependency provides an injector method that will inject the dependency into
any client passed to it. Clients must implement an interface that exposes a setter method that accepts the dependency.

Benefits and Disadvantages of DI
Help unit testing
Extending the application and enable loose coupling
Complex to learn
Compile errors
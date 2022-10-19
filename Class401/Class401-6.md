# Reading notes 10/18/2022

## Random module

- random.randit(0, 5) will cycle through the number 1 through 5

- random.random() * 100 will multiply the values

- random.choice called upon a list will randomly grab an item from that list

- random.shuffle on a list will shuffle the elements in place so they are in a random order

## risk analysis

- The probability of any unwanted incident is defined as Risk. In software testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizizing them to test.

- Why?

>In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

- Risk Identification

>Business Risks: This risk is the most common risk associated with our topic. It is the risk that may come from your company or your customer, not from your project.
>Testing Risks: You should be well acquainted with the platform you are working on, along with the software testing tools being used.
>Premature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required
>Software Risks: You should be well versed with the risks associated with the software development process.

- How to search for the risk

- How to perform Risk Analysis?

- There are three steps:

>Searching the risk
>Analyzing the impact of each individual risk
>Measures for the risk identified

Source: [Edureka](https://www.edureka.co/blog/risk-analysis-in-software-testing/)

## Value of test coverage by Martin Fowler

- Test coverage is a useful tool for finding untested parts of a code base.

- TDD is important, but people should not force a percentage of testing, it is more important to right quality tests then to have 100% coverage of codebase with poor quality tests.

= People focus on coverage numbers too much and instead should focus on making quality tests. Sufficiency of testing is much more than just a percentage of codebase covered by tests.

- You are doing enough testing if:

>You rarely get bugs that escape into production, and
>You are rarely hesitant to change some code for fear it will cause production bugs.

-Source [MartinFowler](https://martinfowler.com/bliki/TestCoverage.html)

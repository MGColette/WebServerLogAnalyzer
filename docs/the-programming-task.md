# The Programming Task

The task is to parse a log file containing HTTP requests and to
report on its contents. For a given log file we want to know,
* The number of unique IP addresses
* The top 3 most visited URLs
* The top 3 most active IP addresses


Chosen Tech:
* Java
* JUnit
* Jacoco for test coverage
* slf4j


## Assumptions and thoughts
* Most active URLs - made 2 assumptions here
    1. take the whole url without extracting the domain
    2. extract the `http` out of url
* Think about :
    1. when the data / logs getting bigger, what are the solution to this?
    2. when the http methods are also including POST, PUT, DELETE? (Used Regex pattern matching)
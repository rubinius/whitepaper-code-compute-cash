# The Rubinius Microservices Platform

_(Note: the features described in Part 3 are works-in-progress with varying degrees of functionality.)_

The Rubinius microservices platform is an implementation of microservices as defined in [Part 2](solution.md), and is composed generally of the virtual machine and the microservices infrastructure.

The Rubinius virtual machine can be used independent of the microservices infrastructure that the platform implements, but the machine's design is extensively influenced by the context of distributed applications.

## Platform philosophy

The goal of the design is fluid access to the power of computation with as few limits as possible being imposed external to the problem being solved.

Unless the problem itself dictates it, a person should not be forced, when starting to work on a problem, to choose a programming paradigm (e.g. object-oriented versus functional), a deployment artifact (e.g. machine-code executable versus bytecode for a virtual machine), a binding strategy (e.g. static versus dynamic typing), or even an instruction set architecture (e.g. register vs stack instructions).

The problem rarely, if ever, dictates these decisions and during development, the priorities that would influence a decision can continually shift. Exploration of a solution never follows a linear path, but rather moves between aspects of the problem, between levels of detail, and between degrees of completeness. Regression and revisiting are common and expected as the problem is defined and understood.

Tools to help understand the problem are as important, or more important, than the particular code that may exist at a moment in time. Language itself is considered the pinnacle of tool creation.

## Interface to computation

### Instruction set

Instruction Set

CodeDB

### Managed memory

Managed Memory Objects and Heaps

### Concurrency

### Diagnostics

Diagnostics, Metrics, Logging

## Platform components

## Platform as marketplace

Interoperability

## Summary of the platform

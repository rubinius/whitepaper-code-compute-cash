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

The Rubinius virtual machine is conceptualized as the user interface to computation. More than just being the mechanism for running code, the idea of "affordance" from user-interface and user-experience design is also relevant.

At the most basic level, the virtual machine aims to blur the distinction between the time code is written and the time it is executed. This is critical because exploration of a solution often requires developing and deploying code in repeating cycles.

The cost of completely developing the solution and then deploying it is prohibitive. Just enough to successfully complete a task is necessary, and then is refined based on the interplay of the problem and the person using the application.

### Instruction set

The instruction set is designed to provide a rich expression of a particular language in the instruction set, which is an intermediate representation that provides the basis for refinement in a particular context.

This explicit role of the instruction set contrasts with typical approaches that attempt to find a set of orthogonal instructions of a uniform, fine granularity and often discard "irrelevant" details that a later subsystem, like the just-in-time (JIT) compiler must re-synthesize.

The instruction set is also designed to be translated to a different system without the rest of the supporting components of a particular virtual machine. This requires that all semantics of the system be transparently implemented purely via instructions, no "primitive intrinsics" are permitted (as that would require also translating the primitives to a different system).

The instruction set is comprised of the following categories of instructions:

1. generic stack instructions;
1. register instructions;
1. branching instructions;
1. concurrency instructions;
1. POSIX system call instructions;
1. managed object lifetime operations;
1. assertion instructions that do not mutate state but can halt;
1. instrumentation instructions that do not mutate state but can emit information;
1. parsing expression grammar (PEG) instructions;
1. method and function resolve / cache / invoke instructions.

The register instructions include those for performing typical arithmetic on machine integers and machine double floating point values.

The instruction set is also designed to enable producing native machine code executables from managed code.

The code itself is stored in the CodeDB, a physical and logical structure that enables lazily loading code at the moment it will be used, as well as associating arbitrary dimensions of information with each executable context, including type information, runtime code coverage, runtime profiling, runtime measurements, exception types, and call graphs.

### Managed memory

The instruction set is one side of the coin, while managed memory is the other. Managed objects can be stored in three types of heaps:

1. the _globally accessible_ heaps that allow arbitrary references between objects in that heap;
1. _closed_ heaps that permit references out to the global heaps but no incoming references; and
1. _isolated_ heaps that do not permit incoming or outgoing references (all references are internal).

The heap configuration allows for a generation garbage collector, as well as parallel and independent collection of isolated heaps

The managed objects are either object-oriented, including a class reference and instance variables reference in the object, and data-oriented, which are only a header and fixed number of bytes per type with a possible internal structure (i.e. set of fields).

The hybrid managed object structure enables object-oriented methods and data-oriented functions to coexist on equal footing, neither being subordinated to the other.

### Concurrency

The virtual machine structures are thread-safe without a global lock, and native operating threads can be created and manipulated by running code. Certain virtual machine tasks also make use of threads.

### Diagnostics

Diagnostics are included in all major components of the virtual machine, and these are emitted as JSON concurrently while the virtual machine is operating.

In addition, various monotonic counters are also included in the virtual machine, as well as via specialized instrumentation instructions.

All virtual machine operations also perform logging of relevant events, and the same logging mechanism is exposed to managed code so that a process has a single uniform log.

## Platform components

There are three kinds of services:

1. _client endpoints_ that expect to receive arbitrary requests, some of which may require proper authorization after an authentication procedure;
1. _service endpoints_ that _only_ receive authorized requests based on a prior, explicit connection between services established via a management protocol; and
1. _data services_ that perform function-oriented data manipulation, either for a single service (client or service endpoint) or as a connection between two or more services.

A client or service endpoint may have a database, but is not required to. A data service does not have a database, but only operates on the databases for which it has explicitly been granted authorization.

## Platform as marketplace

Much of the infrastructure for applications today are open source, from operating systems to programming languages to libraries and frameworks. But open source is an extremely exploitative ecosystem.

Companies benefit extensively, but rarely compensate creators of the source code. The vast majority of contributors see no reward for their effort. Moreover, people from economically disadvantaged or under-represented groups are excluded because they lack the time to devote to unpaid work.

For individual creators, there is little opportunity to make a reasonable amount of money unless the library or system they make is just the right size to mostly exclude competition and for businesses to consider it valuable enough to go through the hassle to purchase. These types of projects are rare. The next step up is a full-blown business with multiple employees in either B2C or B2B categories.

## Summary of the platform

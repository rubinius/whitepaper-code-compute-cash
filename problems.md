# Problems With Software Development And Delivery

The term "software crisis" was coined nearly five decades ago and shows no significant signs of abating.[^3]

#### Misunderstanding Value

Code is a liability, not an asset. The code itself should be discarded at the earliest opportunity. The focus of a business should be replicating, transmitting, and refining what it is learning. DNA carries genetic information, but it is the expression of those genes that has value. Similarly, code may be the carrier of the firm's information and learning, but it is the running code that provides value.

#### Software Construction Is Not Distributed

Today, any interesting piece of software is talking to other software on a separate physical device. This was not true of most software a few decades ago. That is to say, the boundaries of software are less distinct, and software is inherently distributed.

To illustrate the first point, if this program talks to software that is essential to its functioning, is that software a part of the program?

#### Poor Adoption Of Technology Advances

The data supporting the use of DevOps to drive favorable business outcomes is well established, but many firms consider adoption to be optional or have not even considered it. Beyond leaving money on the table, this negligence could threaten the existence of many of these businesses.

#### The General-Purpose Myth

The belief that a single programming language is suitable for almost any task is widely held with an unquestioning certitude that goes beyond advocacy to dogma. There are several consequences of this myth:

  1. Enormous expenditure to create a general purpose programming language and ecosystem;

  1. Significant disincentive to share critical pieces of infrastructure between ecosystems because it is difficult to do so or because the language should be capable of the tasks and maintenance favors the ecosystem's own language;

  1. Enormous cost to advance a system written in one language by rewriting it in another general purpose programming language; and

  1. Inefficient transfer of learning as each separate general purpose programming language ecosystem relearns, for example, how to do concurrency effectively.

The cost of a single general purpose programming language runs into the hundreds to thousands of human-years of effort. The inefficiency of transferring learning and the cost of duplication are notable aspects of the general purpose language myth, but are so widespread in general that they require their own topics.

#### Widespread And Inefficient Duplication

In the past ten years, at least eight new programming languages or systems have come into popular use.[^4] Every one of these languages requires a component for managing software packages written in that programming language. None of them share this component.

And that is just the packaging system, which often competes with the packaging system provided by the operating system. But there are many additional components that are duplicated for every language, including the parser, compiler, optimizer or just-in-time (JIT) compiler, debugger, profiler, and code linter or analyzer.


#### Failure To Exploit Learning

Use of concurrency and approaches to building distributed systems.

#### Lack Of Ecosystem Diversity

The dominance of the infrastructure-as-a-service market by Amazon AWS, Google, Microsoft, and DigitalOcean are visible to everyone, but lack of diversity in the ecosystem extends everywhere, from chip manufacturers to programming languages to operating systems to software libraries.

The lack of diversity is exploited for their own benefit by the dominant players, but the ecosystem suffers from

#### Dysfunctional Open-Source Ecosystem

Broadly, open source is an exploitative ecosystem. The majority of the creators of open source do not capture any value from the ecosystem, and the vast majority of those who profit by using open source do not incur any cost from their use of open source.

#### Centralized Control Of Computation

Those in control serve their own interests, without exception.

#### Location-Based Addressing

One of the worst flaws in the existing structure of the internet is the coupling of trust with a particular machine address.

#### Economic Exploitation

The business models of Facebook and Google are fundamentally rooted in farming people, extracting attention, and mining data that they do not own.

#### Wrong Granularity For Collaboration

The granularity of applications is significantly too course, while the granularity of traditional packages of code, software libraries, is too fine. The necessary level of granularity to support effective collaboration is the elusive software component, something that roughly mirrors today's microservices.

#### Software Architecture Does Not Match Internet Of Things (IoT)

The internet of things exists and is growing daily. Its fundamental nature is massively distributed and vastly networked.

---

[^3]: [The software crisis](https://en.wikipedia.org/wiki/Software_crisis)
[^4]: Clojure, Scala, Ruby, Elixir, Rust, Go, Node, Swift, Haskell.

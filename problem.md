# The Problem of Using Information in a Competitive Market

What is the essential property of information that should dictate how we build digital products?

Let's explore that question by comparing it to material manufacturing.

Imagine that you are the CEO of manufacturing company. I tell you I'm opening a factory, but  instead of using an assembly line, I use a random placement of workstations and a routing algorithm that maps a path from a delivery bay to a workstation for some raw materials, and then from workstation to workstation before arriving at a shipment bay.

What would you say and why?

A moment's reflection will hopefully produce two important realizations. The answer should be definitive, and it derives from facts about the properties of matter as understood by physics. These two are distinct, for definitive answers that flow from an authority, like religion, need have no basis in fact.

Three facts about matter dictate the structure of an assembly line:

1. Two pieces of matter cannot occupy the same place at the same time;
1. Pieces of matter must be spatially very close to affect one another in a controlled way;
1. Order of operations on a piece of matter are crucial for the outcome.

These facts determine the essential requirement of an assembly line, the coordination in space and time of pieces of matter to produce the desired result at the lowest cost. Any alternate structure must be as good or better at coordination.

The assembly line captures the invariants of material manufacturing. It is a ubiquitous structure for that reason. While there is infinite opportunity to improve the particular implementation of an assembly line, its essential structure and function are fixed.

Has this comparison illuminated our original question? At minimum, it should force us to wonder whether matter and information are fundamentally the same.

Let's return to the question in a moment. To get the most out of the content below, a distinction is necessary.

There is a difference between a _problem_ and a _mess_. A mess can get in our way, waste our time, or obscure something useful. We do need to clear the messes, but not get sidetracked by them. There are a lot of messes in the way we currently build digital products, and we will examine these. But the problem is the thing we must understand, and that will enable us to clear the messes. If we get lost in the messes, we'll never understand the problem.

## Information is not matter

Information is an emergent property of a particular configuration of matter.

Consider _wetness_ as an analogy. When water molecules are highly energetic, they are a gas. They are not wet. When they are in a crystalline structure, frozen solid as ice, they are not wet. But when they are in a liquid state, they have this property of wetness. The water molecules don’t change. Wetness is a property of their configuration.

The same pieces of matter can represent different information merely by changing their configuration.

Digital information can be copied with absolute precision using very little energy by causing other pieces of matter to have the same configuration, and without disturbing the original configuration. Information can be copied great distances in a fraction of a second by transmitting light or electric charges. When digital information is copied, the original and the copy are identical.

Information processing fundamentally involves copying information.

In contrast, copying material objects requires enormous amounts of energy. In fact, we cannot really copy them. We must get new material and use processes to manufacture another object. The two objects are not identical.

## The fundamental problem is access to information

The fundamental problem of material manufacturing is _coordination_, which is dictated by the properties of matter. The necessity of coordination goes beyond the structure and function of an assembly line into our processes for _status_, _testing_, and _delivery_. We will revisit the latter idea in the messes below.

What is the fundamental problem of information?

The value of information is using it to make a _decision_, to choose an alternative that has a better outcome. A table just sitting there can be of great use. Information not applied to a decision is either irrelevant or akin to a piece of matter.

In place of coordination, the problem is getting information to the place and time of a decision. _Access_ to relevant information at the moment of decision is essential.

## Important properties of information

As identified above, it is properties of matter that dictate the importance of coordination for manufacturing and the essential structure and function of the assembly line.

What properties of information dictate the importance of access for information and can be used to identify the essential structure and function of a mechanism for building digital products?

1. Information must be used and is valuable in proportion to its ability to produce a more desirable outcome than an alternative.

1. Information takes time to propagate. The time is proportional to the distance between where information originates and where it is applied to a decision, and the resistance in the system to the flow of information.

1. The distribution of information is non-uniform due to the time required to propagate.

1. Applying information implies change, either something that did not exist before, or something different than it was before. The change implies a cost.

1. There is resistance to the flow of information because of the cost of change. Work is required to apply information.

1. Information can be contradictory. Resolving the contradiction requires (possibly) generating and (at least) applying new information.

1. Different amounts of information may be suitable for completing a task. This contrasts markedly with matter. For example, a bottle with a hole in the bottom is not suitable for containing liquid, but decades of car manufacturing illustrate how we may complete a process and yet have immense room to improve the process and result.

1. The value of information degrades over time. As information becomes uniformly distributed, it becomes background, and change from that background implies applying new information. This process appears effectively infinite. A functioning car from fifty years ago will provide useful locomotion, but it won't compete in the market or on performance with a car built today. There is no vintage information.

These properties are inter-related and interact, but do not appear reducible. There are both individual effects and systemic affects. The time to propagate is both a limitation of a signal (i.e. the speed of light) and a result of systemic resistance. The systemic resistance is partly due to the cost implied by change, but also related to non-uniform distribution. If I have sufficient resources and great determination but haven't receive the information yet, no effect is possible.

We apply information to build digital products whose value derives from applying information. We are tool makers. In material manufacturing, tool makers are a subset of all manufacturing. For digital products, the tool makers are a superset of all digital products.


## Messes made misunderstanding information


The term "software crisis" was coined nearly five decades ago and shows no significant signs of abating.[^1]

#### Misunderstanding Value

Code is a liability, not an asset. The code itself should be discarded at the earliest opportunity. The focus of a business should be replicating, transmitting, and refining what it is learning. DNA carries genetic information, but it is the expression of those genes that has value. Similarly, code may be the carrier of the firm's information and learning, but it is the running code that provides value.

#### Software Construction Is Not Distributed

Today, any interesting piece of software is talking to other software on a separate physical device. This was not true of most software a few decades ago. That is to say, the boundaries of software are less distinct, and software is inherently distributed.

To illustrate the first point, if this program talks to software that is essential to its functioning, is that software a part of the program?

#### Poor Adoption Of Technology Advances

The data supporting the use of DevOps to drive favorable business outcomes is well established, but many firms consider adoption to be optional or have not even considered it. Beyond leaving money on the table, this negligence could threaten the existence of many of these businesses.

#### The General-Purpose Myth

the idea of whole (coherent) enough to complete a task. one of a kind, custom, general purpose, specialized

The belief that a single programming language is suitable for almost any task is widely held with an unquestioning certitude that goes beyond advocacy to dogma. There are several consequences of this myth:

  1. Enormous expenditure to create a general purpose programming language and ecosystem;

  1. Significant disincentive to share critical pieces of infrastructure between ecosystems because it is difficult to do so or because the language should be capable of the tasks and maintenance favors the ecosystem's own language;

  1. Enormous cost to advance a system written in one language by rewriting it in another general purpose programming language; and

  1. Inefficient transfer of learning as each separate general purpose programming language ecosystem relearns, for example, how to do concurrency effectively.

The cost of a single general purpose programming language runs into the hundreds to thousands of human-years of effort. The inefficiency of transferring learning and the cost of duplication are notable aspects of the general purpose language myth, but are so widespread in general that they require their own topics.

#### Widespread And Inefficient Duplication

In the past ten years, at least eight new programming languages or systems have come into popular use.[^2] Every one of these languages requires a component for managing software packages written in that programming language. None of them share this component.

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

It was never a requirement of the Internet that people be the ones connected to it. In fact, people have never been connected to the Internet. It has always been machines. In the future, people may connect to the Internet via a direct neural linkage, but for now it will continue to be machines.

The Internet of Things (IoT) is both old and new. Its fundamental nature is massively distributed and vastly networked. The things connected to the Internet may be interfaces for people, artificial intelligences, autonomous agents, sensors, or other machines.

[^3]

---

[^1]: [The software crisis](https://en.wikipedia.org/wiki/Software_crisis)
[^2]: Clojure, Scala, Ruby, Elixir, Rust, Go, Node, Swift, Haskell.
[^3]: [Radical new vertically integrated 3D chip design combines computing and data storage](http://www.kurzweilai.net/radical-new-vertically-integrated-3d-chip-design-combines-computing-and-data-storage)

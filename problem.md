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

1. Work is required to apply information because it causes a change, either something that did not exist before, or something different than it was before. Work implies a cost, and that causes resistance to the flow of information.

1. Information can be contradictory. Resolving the contradiction requires (possibly) generating and (at least) applying new information.

1. Different amounts of information may be suitable for completing a task. This contrasts markedly with matter. For example, a bottle with a hole in the bottom is not suitable for containing liquid, but decades of car manufacturing illustrate how we may complete a process and yet have immense room to improve the process and result.

1. The value of information degrades over time. As information becomes uniformly distributed, it becomes background, and change from that background implies applying new information. This process appears unbounded. A functioning car from fifty years ago will provide useful locomotion, but it won't compete in the market or on performance with a car built today. There is no vintage information.

These properties are inter-related and interact, but do not appear reducible. There are both individual effects and systemic affects. The time to propagate is both a limitation of a signal (i.e. the speed of light) and a result of systemic resistance. The systemic resistance is partly due to the cost implied by change, but also related to non-uniform distribution. If I have sufficient resources and great determination but haven't receive the information yet, no effect is possible.

We apply information to build digital products whose value derives from applying information. We are tool makers. In material manufacturing, tool makers are a subset of all manufacturing. For digital products, the tool makers are a superset of all digital products.

The principle problem of access to relevant information at the moment of deciding, which derives from the properties of information described above, requires a mechanism for building digital products that is like the assembly line for manufacturing. That mechanism is _microservices_.

To fully understand the value of microservices, it's necessary to reflect on the messes we create when we misunderstand the probem of building digital products.

## Messes made misunderstanding information

The term "software crisis" was coined nearly five decades ago and shows no significant signs of abating.[^1]

Common symptoms of the software crisis include projects that exceed predicted timelines and budgets, software that fails to meet quality standards or fails to function as expected, and systems that require enormously greater resources to maintain than predicted.

These messes can be roughly grouped into three areas:

1. Misapplication of manufacturing processes to building digital products;
1. Failure to exploit existing, available knowledge; and
1. The myth of the general-purpose programming language.

### Misapplying manufacturing processes to digital products

Everywhere that digital products are built, businesses have applied material manufacturing processes to building them. But matter and information have different fundamental problems. Misapplying manufacturing processes causes far higher costs by wasting resources on unnecessary activities or delaying the value that could be generated.

_Digital products require different processes from those used for material manufacturing._

In manufacturing processes, _status_, _testing_, and _delivery_ are so critical to the successful outcome that they constitute a huge portion of the total cost.

The question, _"What is the status of this?"_ is important because of the need to coordinate many things to get pieces of matter to arrive at the same place and time.

Acquiring matter and moving it around requires a lot of energy. Since no two pieces of matter can occupy the same place at the same time, coordination errors can be extremely costly. Also, idle machines and workers are wasted resources.

The need for testing is imposed on material manufacturing by the properties of matter. Testing must be performed before manufacturing so that correctness is confirmed. "Does this piece connect to this other piece within the manufacturing tolerances and in a way that results in the completed component functioning correctly?"_ This must be right beforehand because it is extremely costly to change after starting manufacturing.

Finally, the product must be delivered to the customer intact and working correctly. Transporting the product is costly, and the customer must be satisfied, or they will return the product and the cost of the product and cost to process the return are wasted resources.

In manufacturing, the need for _coordination_ underlies the processes for status, testing, and delivery,

Why is coordination nearly irrelevant in digital products?

Consider a Tesla car. Two examples are the autopilot feature and the battery capacity. These are software updates. The hardware has the capability, but whether that capability is accessible is determined by some value in the software.

We can generalize this to _any_ feature in a digital product.

An enormous amount of information can essentially occupy the same place at the same time. We can deliver features that are not enabled yet, or we can simultaneously deliver multiple alternative features in a single application, and determine at the moment of interaction which will be used.

In a digital product, at any moment, we can create a feature _that completes a task_ with some degree of functionality, and then refine that repeatedly without needing any other coordination or disturbing the rest of the system in any way.

This is similar to the process of building a bridge across difficult terrain where an initial, lightweight string of material is passed across, that’s used to pull across a heavier, more capable wire, and that’s used to bring across something more useful, and so on.

Using this process of refinement, we can integrate with a remote system we do not control with almost no coordination, or with the cost of any necessary coordination being extremely low.

Since coordination is not imposed on building digital products like it is in material manufacturing, the need for status nearly disappears. But more importantly, _the digital product itself is the status_. Requiring status updates as an artifact independent of the digital product adds cost without value.

What about testing? Without the need for coordination, the requirement for testing at a privileged point in time, before manufacturing, is eliminated as well.

Correctness in a digital product is not a unitary property, completely true at a moment in time. One feature may be correct and useful while another is not. Correctness may also be refined over time. The changes can be localized to part of the product so that their cost can be minimized.

_Correctness becomes a function of the digital product, not something that can be asserted beforehand._

Digital products interact with people and other agents beyond the control of those building the products. That interaction requires specifying boundaries of correct behavior and constantly monitoring and adjusting the system to maintain those invariants.

Now, consider delivery. Nearly every digital product is, or will be, delivered almost instantly at the moment it is used. Once the infrastructure is built, there is almost no coordination at the point of use, much like turning on a light switch and using electricity.

Digital products do not require the same manufacturing processes of status, testing, and delivery, but they do require processes to minimize their cost. We will examine those necessary processes in [Part 4](benefits.md)

### Failure to apply existing knowledge

Lacking any theory of "applied information", advocating for one process instead of another when building digital products devolves to an appeal to power, fame, or fashion. Either the decision is made by someone who wields the most power, or by following the advice of the most famous person, or by whatever happens to be of most interest to people at the moment.

This state of affairs should deeply concern us, but as builders of digital products, we are not alone. Renown physicist, Sir Roger Penrose has written a book titled, _Fashion, Faith, and Fantasy in the New Physics of the Universe_. However, just because we are in good company shouldn't lessen the urgency to find firmer intellectual ground.

The messes we create because we don't have a good theory tend to perpetuate the messes much more than they encourage developing that theory. They form a reinforcing loop of negative outcomes where the frustration caused by our inability to solve the "software crisis" adds fuel to the effort to "find something that works". The current appeal in some circles to "software craftsmanship" reflects the confusion. John Day has been highly critical of the same lack of theory development in the domain of networking broadly and the Internet in particular.[^2]

Numerous approaches have been offered to improve the quality, efficiency, and predictability of software, including Waterfall, Agile, Scrum, Lean, and DevOps. Some of these approaches blend elements from the others. The approaches have _evangelists_ who interpret the approaches for the masses, weigh in on correct applying them, and attempt to convert companies to the approach. Sometimes the results are measured, but if that's too difficult, it's acceptable to cite anectdote as pursuasive evidence.

Either it's true that any possible approach to building digital products is as likely to be as effective, or there is a reason to use one approach instead of another. The inability to justify using an approach based on outcomes that can be independently predicted by theory and verified prevents us from learning from advancing knowledge.

It should be apparent that matter and information differ. If manufacturing processes are not transferable to building digital products, we should wonder what structure and processes are required. Until we understand that, we will continue making messes.

### The general-purpose myth

The evolution of all products follows a predictable path. First there is no product, but there is a need for completing some task. Then there is a one-of-a-kind, like the first Wright brothers airplane that flew. Then there are custom products that built one-at-a-time. Following some standardization, there is a relatively general product that can be mass-produced.

The mass production, econmies of scale stage is often seen as the pinnacle of manufacturing. But there is a stage beyond it. Mass production implies a generalization within some acceptable tolerance. Beyond mass production is the _specialized_ product. This stage efficiently produces variations that have value beyond the generality of mass production.

The belief that a single programming language is suitable for almost any task is widely held with an unquestioning certitude that goes beyond advocacy to dogma. There are several consequences of this myth:

1. Enormous expenditure to create a general purpose programming language and ecosystem;

1. Significant disincentive to share critical pieces of infrastructure between ecosystems because it is difficult to do so, or because the language should be capable of the tasks and maintenance favors the ecosystem's own language;

1. Enormous cost to advance a system written in one language by rewriting it in another general purpose programming language; and

1. Inefficient transfer of learning as each separate general purpose programming language ecosystem relearns, for example, how to do concurrency effectively.

The cost of a single general purpose programming language runs into the hundreds to thousands of human-years of effort.

In the past ten years, at least eight new programming languages or systems have come into popular use.[^3] Every one of these languages requires a component for managing software packages written in that programming language. None of them share this component.

And that is just the packaging system, which often competes with the packaging system provided by the operating system. But there are many additional components that are duplicated for every language, including the parser, compiler, optimizer or just-in-time (JIT) compiler, debugger, profiler, and code linter or analyzer.

The general purpose myth permeates every corner of digital products because code has a central role in all the systems. The current boundaries around a working system encompass so much code that a single language is required, even if not desired.

The resistance to change baked into digital products compounds the cost of interoperability and virtually guarantees that using a different programming language in the product will force rewriting large portions of code, or struggling with brittle, nearly impermeable boundaries between parts implemented in different languages.

All of the effects of the general purpose myth raise the cost of sharing and adopting advances in knowledge.

## Summary of the problem

Access to relevant information at the moment of making a decision is the fundamental problem of working with information, both when building digital products and when using them.

Manufacturing processes suited for the problem of coordination that is dictated by the properties of matter add unnecessary cost when applied to building digital products.

However, based on the existence of the assembly line for manufacturing, we should expect that a structure and process for building digital products exists.

Developing such a structure requires understanding the properties of information and developing a suitable theory that will predict the outcome of taking one approach instead of another.

Without developing theory, we will remain limited by the messes we create when applying _ad hoc_ attempts to find, in John Day's words, "something that works".

In [Part 2](solution.md), we examine a structure and process for building digital products.

---

[^1]: [The software crisis](https://en.wikipedia.org/wiki/Software_crisis)
[^2]: Personal correspondence and _Patterns in Network Architecture_, John Day, Prentice Hall, 2008
[^3]: Clojure, Scala, Ruby, Elixir, Rust, Go, Node, Swift, Haskell.

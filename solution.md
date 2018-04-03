# Microservices are the Digital Assembly Line

> "A field cannot consider itself a science until it can progress beyond natural history; moving from describing what is, to positing principles or theories that make predictions and impose constraints."[^1]

Microservices are computational processes that communicate with other such processes as peers in a networked graph. This is a _system_ definition. The processes themselves, their communication, and the graph in which they are embedded, are essential and inseparable.

## Structure of microservices

Microservices are fundamentally a form of _distributed application_ with certain constraints.

As emphasized above, microservices are a system. Often something tangible can help us begin to disentangle a system definition. Since "service" evokes the idea of an object we can observe, let's begin with the question, _"What is a service and how big is it?"_

The question of size is common because microservices are often contrasted with a "monolithic" application, and these tend to be very large.

The question of size, while relevant, is not what determines what a service is. The answer isn’t a particular number of lines of code, or number of routes in an API endpoint, or functions in the process. By answering, "What is a service?" we will answer the question "How big is it?" as well.

There is concept that we will find repeatedly in microservices, the idea of _coherence_,
One of the definitions of coherence is, "the quality of forming a unified whole."

Consider a biological cell. A human cell is about 200 times bigger than a bacterium. While both kinds of cells are functional, the difference in size is a couple orders of magnitude, but in each case, the cell is a whole structure.

Similarly, a _service_ in microservices is a component with coherence.

To illustrate the idea of coherence, here’s an example I learned from David Snowden (creator of the [Cynefin framework](https://hbr.org/2007/11/a-leaders-framework-for-decision-making)).

Imagine that you wake up in the morning and look outside. Overnight it has rained. In the bushes, you see a web that was spun before the rain and has been damaged by the rain. You can see enough of a structure to recognize it as a spiderweb despite the damage, and not just some strands of spider silk. At what point would the spiderweb cease to be a web?

Given the definition of coherence and the illustration above, we see two boundaries: enough to be a whole, and less than what would be _more than a whole_.

If there is obviously something missing, that particular service is not big enough, it lacks coherence. If, on the other hand, you can see an internal boundary around something that can be identified as a whole, it’s too big.

Despite starting to define "service" as a concrete object, it is a logical component. The concrete objects in microservices are _processes_ running on a computer, the network connecting the computers, and the messages exchanged by the processes.

A service may be more than one process that is running identical code and receiving messages behind a proxy that may perform load balancing. To any other service communicating with this one, it is entirely transparent whether the service is composed of a single process or more than one process.

After examining the basic properties of microservices, we will revisit the definition of a service to better understand it in relation to the system in which it is embedded and to which it contributes.

## Basic properties of microservices

There are four essential properties of microservices:

1. _Substitutability_: the ability to substitute one subgraph for another to provide an alternative that maintains or extends functionality for one part of the network graph, while not diminishing it for any other part;

1. _Replaceability_: the ability to replace one subgraph with another for every part of the graph that communicates with that subgraph;

1. _Isolation_: any process in the graph only has an effect on the system as a whole by means of the communication it performs. Nothing happening inside a process can otherwise change the state of the system; and

1. _Repeating structure at different scales_. This is a common attribute of complex systems, and is referred to as fractal, or self-similar at different scales.

Substitutability and replaceability are not equivalent! Substitution can provide an alternative path of evolution for a part of the application (imagine a fork in the road and both paths are taken), while replacement converges back to a single path for the entire application.

Isolation should not be confused with some sort of immutability. For example, a particular process may be a clock, with its internal state changing with a periodic regularity, but the effect of that change is only visible when that process communicates.

The property of isolation helps clarify the role of a process. A process must be programmed with the constraint that more than one instance running concurrently must not change the property that the number of processes comprising a service is transparent to any service that communicates with it.

These four properties give microservices tremendous power.

Consider a graph of three services: A, B, and C. A and B communicate with C. Due to substitutability, isolation, and repeating structure, we could replace C with a complete graph of new services behind a single service (playing a role like load balancer or proxy) that conforms to the behavior of the previous service C. From the perspective of A and B, nothing would have changed. This "zooming in" on C to find another graph is what is meant by self-similar at different scales.

At the same time, we could "zoom out" in the neighborhood of the graph embedding A, B, and C, substituting a new service that stands in place of this subgraph.

What is especially powerful is that the concept of coherence is relevant to the attributes of substitutability, replaceability, and repeating structure described above. Due to coherence, we can replace a portion of the graph with another graph and preserve both local coherence and wider coherence across the graph.

The logical nature of service should now be more clear. A service is a _component_ with coherence, and due to the property of isolation, that component may be an individual service or a subgraph of services.

Similarly, an application is a subgraph that provides some coherent functionality. Based on our definition above, a service may be an application in itself.

_**It is this resilience to change that makes microservices so powerful in the context of the process of learning under the constraints of a business.**_

## Microservices are universal

The properties of microservices make them highly compatible with a network of heterogeneous devices, from cloud servers to connected, embedded devices, and sensors in any environment.

In fact, this architecture excels at dealing with this variance of scale. A process running on an 8-bit Arduino can have both the wholeness attribute of coherence, and communicate in a network where it can be provided exactly what it needs by leveraging substitutability. Microservices provide a single unifying architecture.

Since there are no problem domains that are incompatible with the properties of microservices, they are _context-independent_.

Of course, as we scale down, at some point we reach a physical CPU, and that level would not be another recursion into nodes in a graph. But it’s worth noting that Carl Hewitt’s [Actor model](https://en.wikipedia.org/wiki/Actor_model) of computation (which is at least equivalent to the lambda calculus or Turing machine models of computation), where an Actor sends and receives messages, is consistent with the structure of microservices.

As we scale up, there is no limit where microservices become insufficient. A subgraph of a multitude of processes can be represented to another part of the graph as a single node, if that were necessary.

Since system size is not a factor of the essential properties of microservices, the are also _scale-independent_.

By scale-independence, we emphatically do not mean the ability to "scale" a particular application. Microservices have been misunderstood as only suitable when dealing with a large volume of requests or users. This has caused a great deal of confusion.

Adapting to a volume of users or requests is _one problem_ in the entire set of problems that an application may need to address. Other problems may be a bound on the latency of a response, or the volume of responses that can be handled in a particular unit of time, or the total throughput of data in the system, or the rate of change of the system, or the size of the team building the application.

All of these potential problems are examples of the need to apply learning when building an application. They can all be handled using the essential properties of microservices.

## Microservices are optimal

Beyond being independent of context and scale, microservices are transparent to the problem being solved.

The properties, especially substitutability, permit an arbitrarily small local change that does not perturb the existing system but allows for adding new information.

The structure of microservices does not impose additional overhead on the solution to a problem, which maximizes the ability to apply learning to the system. This is not true of other architectures.

For example, consider an architecture that forces a certain minimum cycle time, like deploying once a week. The additional cost of coordination to meet that constraint has no value to the solution. It is pure overhead. In this way, that more limited architecture is _not_ transparent to the problem.

Any system that has the same properties described here, and does not impose additional constraints on the solution to a problem, is equivalent to microservices.

To be a _superior_ architecture for the basic problem of working with information, a system would need to provide greater leverage for applying new information, or further reduce the cost of applying information.

This is exactly the case we saw for the assembly line in manufacturing. Microservices are universal and optimal. They are a necessary and sufficient structure for building digital products.

In [Part 4](), we will examine the costs of building microservices infrastructure, and the effect microservices will have on existing businesses, including cloud providers.

## A process for working with microservices

As detailed in [Part 1](problem.md), one of the biggest messes we make building digital products is caused by applying manufacturing processes to information.

The properties of microservices illuminate both a structure _and a process_ that is consistent with the properties of information.

Here again we encounter the idea of coherence, in this case, the idea of whole enough to complete a task.

The holistic approach builds a complete task in the simplest way and then refines it as information is created or becomes available. It is a fundamental process for working with information because it helps identify and eliminate uncertainty due to missing information that can hide costs.

To support the holistic approach, there are three necessary measurements: 1. batch size; 2. cycle time; and 3. quality of feedback loops.

These three measurements monitor how well the system is processing new information, and provide notice when intervention is necessary.

_Batch size_ is a measure of the amount of stuff that must be coordinated as a unit that is moving from one stage to another in your process. This can be measured at a point in time (how big is this batch) and over time (what is the average batch size).

_Cycle time_ is the time it takes to complete one pass through your process.

_Quality of feedback loops_ is a measure of necessary information being available at the point a decision needing that information is made.

These measurements are actionable. A batch size that is tending to drift larger may have many causes that may require analysis, but the effect (batch size) is unambiguous.

To build digital products, we use the end-to-end approach and monitor batch size, cycle time, and the quality of feedback loops to control the overall process of learning the cause-and-effect relationship for generating value.

## Summary of the solution

Microservices are a structure dictated by the properties of information.

Like manufacturing and the assembly line, microservices are the lowest cost solution the critical problem of access to information at the moment of making a decision, both in the process of building digital products, and for the digital products themselves as they are used by people as they solve problems.

Further, the structure of microservices dictate the process for building applications.

In [Part 3](platform.md), we describe the Rubinius virtual machine and infrastructure for microservices.

---

[^1]: Chapter 1, _Patterns in Network Architecture_, John Day, Prentice Hall, 2008

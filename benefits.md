# Benefits of a Microservices Platform

Microservices are a structure for digital products that solves the constraints imposed by properties of information.

The benefits of microservices derive from the leverage the structure provides to build digital products and the enormous potential to reduce costs, both by virtue of the efficiency inherent in the platform and due to the standardization that is possible.

The structure of microservices dictate the processes that are used to build digital products, and exert significant influence on the organization of businesses.

The standardization that is possible extends deeply inside the traditional boundaries of a business, which will both disrupt existing structures, as well as make new structures economically viable.

## Structure of digital products

Digital products, often called _applications_, will be built on microservices infrastructure.

The structure of microservices dictate the fundamental architecture. This eliminates the role of "architect" in building digital products. The focus shifts to building services that can be composed in novel ways to solve problems.

The more visible intesection of problem and solution ensures tighter collaboration between the roles in a business, from business strategy to product owner to marketing to sales, and obviously, software development. These roles now collaborate around ever refined solutions (drawing on the coherence property) in a series of dialogs, rather than the failed mimicry of an assembly line delivering a manufactured product.

The transition to microservices infrastructure represents the industrialization of building digital products. Unsurprisingly, it has both advocates and detractors. One of the arguments against microservices is that there is significant costs to building them.

The current structures visible around us are a hydrid of various structures, and the situation is similar to the period of transition from steam engines to electric motors as the industrial revolution was gaining momentum.

There was an extensive intellectual debate whether a single electric motor or multiple electric motors per factor was the better solution. In retrospect, it seems absurd that there was such a debate, but at the time, the value of multiple electric motors was far from obvious.

Just as there is a cost to build an assembly line, there is obviously a cost to build the microservices _infrastructure_, but this can be done in a standard way and learning can be widely shared. Microservices represent the _minimum_ cost for providing the necessary infrastructure for digital products, from a very small scale up to a global scale.

The biggest flaw in current approaches to microservices is the failure to recognize the opportunity, and tremendous value, of standardization.

The cloud providers, which are focused on enabling arbitrary architectures and workloads, are not building microservices infrastructure. Instead, they are building systems that tightly bind an application to the components the provider makes available. It would require substantial cost to move an application to a different provider. This is merely the next iteration of vendor lockin.

In fact, there is significant similarity between cloud providers and telecoms from before the Internet. In both cases, the "infrastructure" they provide will be commoditized. For telecoms, the rise of packet-switched networks eliminated the need for specialized kinds of hardware and distinguished routes (virtual circuits).

Microservices are a unifying infrastructure that integrates a myriad different devices. The proliferation of IoT protocols and concerns represents a shocking disregard for history (or the interests of some businesses erecting artificial barriers to competition).

The IoT devices merely represent nodes in a graph that have certain QoS (quality of service) requirements. As professor Day has demonstrated in RINA, there is _one_ application protocol and _one_ data protocol. By separating mechanism and policy, a fundamental theory of networking can accommodate all the uses of the Internet.

Unlike manufacturing, microservices can scale down to very small "applications" once the infrastructure is standardized. [Part 3](platform.md) offered one view toward that standardization.

## Process for building digital products

As with structure of applications, microservices dictate the processes we use to build digital products.

Enormous amounts of resources are routinely wasted pursuing processes adopted from manufacturing. Every standup meeting, every status report, every project manager chasing people down for status reports, all the effort to estimate tasks, box things into sprints, and coordinate "releases". These wasted resources represent pure overhead, and eliminating them (and their knockon effects) can represent orders of magnitude efficiency improvements.

Due to misunderstanding that coordination is not required for building digital products like it is for manufacturing, we have been misled us about the value of things like Agile, Scrum, and Lean. Instead of being useful, they are adding irrelevant activities and unnecessary costs.

Of all the popular processes, DevOps has come the closest to justifying itself by studying the correlation of business outcomes with use of DevOps practices. This focus on measurable differences is worthy of praise, but it only the beginning of establishing a scientific approach to building digital products. Correlation is not causation.

We have solid evidence that smaller batch size and cycle time is correlated with lower mean time to resolution (MTTR). But how small is the right size? What happens if we see a contradiction where smaller batch size resulted in higher MTTR?

Without a theory, the case study approach based on correlation can just as quickly devolve to fame, fashion, or power making decisions.

Returning to the properties of information outlined in [Part 1](problem.md), we both see justification for focusing our processes on batch size, cycle time, and quality of feedback loops, but can also predict how we can get counter-productive outcomes when supposedly "doing the right thing" if our actions blindly follow some prescription.

The importance of monitoring the quality of feedback loops is sound precisely because information is valuable when it is available at the point a decision is made.

Small cycle times are necessary because it takes time for information to propagate, and information needs to propagate to be accessible. Small batch sizes are _required_ to build digital products efficiently. Not "desirable", _required_.

Likewise, small batch sizes are _necessary_ to perturb the system as little as possible while still making use of information as soon as possible.

One of the more profound results of understanding the properties of information is recognizing that "coding" is a _process_, not a result. Critically, _all code is a liability, not an asset._

Code is never the product. It is like the truck that delivers a product to the customer. The customer does not care whether that truck is UPS or FedEx, as long as the difference between the two doesn't affect getting the product as soon as possible.

Code _always_ represents imperfect information that is frozen at some point in the past. The code should be disposed of at the earliest possible moment, and replaced with a better solution that represents a better understanding of the problem.

The microservices properties of substitutability, replaceability, and isolation make it possible to replace code as quickly as possible with the least possible disruption to other features.

One element of replacing code quickly is that no resources are wasted trying to convince someone that their code is not performing as needed. Developers don't need to debate which of two approaches are superior when there is not basis to decide. Nor do they need to convince a project manager to allocate time for "paying down technical debt". The granularity of microservices, and the property of substitutability, enable a developer to devote the otherwise wasted time into the effort to build or use a different service that does meet requirements.

In fact, the myth of "technical debt" can vanish. It was never real anyway. It was a consequence of imperfect information applied at a point in the past _when no alternative was actually possible_. It was never a true tradeoff because necessary information wasn't available. The properties of substitutability and replaceability enable eliminating eliminating or improving code with minimal resources devoted to outdated decisions and artifacts.

The venerated MVP will be another casualty of moving to a scientific approach to building digital products. There was never a way to measure either _minimal_ or _viable_.

In place of this rule-of-thumb approach, we substitute the same concept of coherence used to define a service and an application. We focus on completion of a task where we _can_ measure "minimal", which is precisely the inflection point between not completing the task and completing the task. Again, the property of substitutability enables us to disregard all non-essential aspects and focus on the critical task at a moment in time.

To effectively build digital products using microservices will require different, constantly updated, processes in place of those that were erroneously adopted from manufacturing.

Those proceses are not arbitrary and do not need evangelists. They are grounded in measuring real effects (batch size, cycle time, quality of feedback loops), and combined with the standardization enabled by microservices, will enable measuring _efficiency_, the ratio of the useful work performed by the input of resources.

## Security by construction

Security must be an essential element of correctness that permeates every corner of the digital products we build. Securing a product after it is built, for example, by "hardening" the system on which it is running, is an oxymoron. It is not _built_ until it is secure.

Microservices enable securing _every_ communication between systems. In the Rubinius platform, more than "enabled", it is _required_. Further, the authorization is checked before the communication reaches the code running the service. Security is an element of the infrastructure.

A recent trend is particularly relevant here, [Zero Trust Networks](http://shop.oreilly.com/product/0636920052265.do). The idea is simple, there is no longer a privileged boundary (or perimeter) separating "internal" nodes from external ones, and where the internal ones are given a different level of trust than external ones.

That perimeter used to coincide with the boundary of the business, where it controlled the internal nodes but not the external ones. Eliminating that boundary allows rich interactivity, where trust and security are functions of a particular node, not the privileged status due to that boundary.

Beyond communication, the structure of microservices imposes fine-grained boundaries on the data in the system. There is not a "lake" of data just waiting to be exploited. The data in the system becomes a function of the application, not merely something the application operates on.

The containment offered by securing communication and imposing fine-grained boundaries is an important aspect of security, but by itself is insufficient. Security must also be a property of _correctness_ that is constantly monitored and becomes a fluid response by the application in real time.

## Quality by degrees

As hinted at with respect to security above, the _boundary_ of an application becomes indistinct when microservices are ubiquitous. This will be expanded on below, but the implication for correctness is important here.

The quality of an application will be a property of its correctness. The ability to "test" before "delivering" an application will not exist. The inter-dependence of services will mean that substantial portions of the application will not be controlled by the same team or company. Just like security, correctness will be an ongoing, fluid response by the application in real time. Quality will encompass correctness, response to scaling demand, and recovery from errors.

This continual monitoring and embedding of quality in the application has been created in things like the Netflix chaos monkey, but will become an essential and ubiquitous aspect of all applications.

Quality will also be a function of business value. Where additional quality can provide more value, it will be added. This will be measured at such fine granularity that significant waste resulting from overbuilding will be eliminated. The decision whether to use an existing service or build one will be constantly re-evaluated in response to changing circumstances and changing demand. The ability to respond quickly, and at such fine granularity, is built into the infrastructure of microservices.

## A new paradigm for business

The context of microservices is a viable business building digital products. Any business in a market must satisfy a simple set of equations:

**operating cost ≤ captured value < created value**

Create more value for the customer than you charge for your product. Keep the cost of creating that value less than or equal to the money you make from selling your product.

A further constraint is the finite size of the market, even a market that is growing. This forces a business to strive for _competitive advantage_.

A business must find a _cause-and-effect_ relationship between what it does and what the customer needs. The process of finding the cause-and-effect relationship is _learning_: identifying a good explanation that enables new information to replace incorrect beliefs.

Identifying a good explanation requires both producing the explanation, and testing whether it yields a repeatable process for creating business value.

The key metric of a business is _**the rate at which learning is converted to revenue**_.

Because of learning, the value of anything goes to zero over time. In a competitive market, there are three types of businesses:

1. Ones that drive the value of their product to zero at the average rate;
1. Ones that do it faster than average; and
1. Ones that do it slower than average.

Only companies who learn fast enough to drive the value of their product to zero faster than average have a competitive advantage.

The constraints on a business, and the requirements of the principle process of a business, are what make microservices relevant. But what impact will microservices have on the existing business structures?

The economist, R.H. Coase, in his book The Firm, the Market, and the Law says this about the size of a firm (emphasis added):

> In my article on "The Nature of the Firm" I argued that, although production could be carried out in a completely decentralized way by means of contracts between individuals, the fact that it costs something to enter into these transactions means that firms will emerge to organize what would otherwise be market transactions whenever their costs were less than the costs of carrying out the transactions through the market. The limit to the size of the firm is set where its cost of organizing a transaction becomes equal to the cost of carrying it out through the market.

While Coase does not explicitly refer to the firm’s boundary, it is the boundary that determines the firm’s size, which is precisely the number of employees inside that boundary.

Consider the boundary of a digital product, like Twitter. Assume that Twitter runs some of its processes on Amazon AWS and some in its own data center.

You open the Twitter application on your phone and start looking at tweets. You notice one that links to an interesting article in The Washington Post. You tap the link and the article is rendered for you. After reading a few paragraphs, you decide to share it with your friend, so you tap the control and select the option to DM your friend the article. Twitter notifies your friend that you’ve shared a DM, and your friend opens their laptop browser to look at your tweet. The friend clicks on the link and visits the main website for The Washington Post, then decides to share the article in an email to a friend.

Where is the boundary of the Twitter digital product, or the boundary of the Twitter app on your phone? Is the interaction itself part of the app, but not the content it renders? Are the AWS instances serving some content to your phone app part of the phone app? What about the servers for The Washington Post?

In a connected world, determining where the boundary of one thing is starts to become extremely difficult.

Businesses have built "APIs" to permit others to use their digital products in a controlled manner, but microservices encourage rich and extensive interactions. Instead of endlessly duplicating functionality, businesses can transparently provide and use highly standardized, or highly customized services.

The leveling of the field for competition that microservices promotes by driving down the transaction costs will likely erode the size of firms that we see today.

More than just reducing transaction costs, the fine-grained approach that microservices enables will allow much greater variability in the cost of a particular service, and better matching of technical skill to the task required. This is both an opportunity for businesses to reduce costs, as well as an opportunity for individuals providing specialized services.

The advantage for every business is that they will be able to leverage highly standardized services, but this also represents a risk since every business will have the same access. This is not unlike manufacturing today where access to resources is essentially equalized. Despite this, some companies like Toyota consistently outperform peers in the market.[^1]

## Decentralization promotes diversity

The impact that microservices will have on businesses indicates a trend away from the massive centralization that is currently the norm.

Microservices present the correct granularity to support collaboration. Historically, in digital products, collaboration is centered in programming languages, libraries, or application frameworks. None of these adequately solve the problems of collaboration because all of these require additional mechanisms to yield functioning applications.

In contrast, microservices can be offered and consumed with no additional effort beyond that necessary to run the microservices infrastructure. The microservices properties of isolation and repeating structure enable deep collaboration between services running on different instances of microservices infrastructure. The blurring of boundaries described above is a positive influence on collaboration and diversity.

Microservices is not neutral architecture. It favors distribution, decentralization, and diversity. Centralization is only achieved at a greater cost.

Any degree of lessening of centralization is _decentralization_. It is the trend that should interest us. The property of information that makes it infinitely copiable is another force working against centralization.

Decentralization implies, but does not guarantee, more diversity. Decentralization is the only way that diversity can increase.

## A return to human values

There are many sources of conflict in human society, and they all eventually reduce to 1. who benefits? 2. who pays? and 3. who decides? The _supply-demand_ curves are simple representation of the conflict inherent when two parties attempt to maximize a function in opposite directions.

The best _collective_ outcomes are achieved when no _individual_ (whether a person or entity) enjoys undue influence. A continual process of rebalancing and leveling power is necessary to avoid accumulation that tips the system toward pathological outcomes.

As described in [Part 3](platform.md), we can choose to impose constraints to favor _a direction toward_ desirable outcomes and disadvantage undesirable ones. A single highly-dominant provider of a feature in a large market diminishes the overall benefit possible by adding monocultural vulnerability while limiting potential benefit from variations. Setting an overall disposition on the evolution of the system allows beneficial outcomes globally without dictating outcomes locally.

The properties of microservices maximize applying new information. This inherently limits any attempt to consolidate control because the balance is heavily tilted toward replacing any component that begins to assert control at the expense of the ecosystem.

## Summary of the benefits

Just as the assembly line significantly reduced the cost of manufacturing, microservices provide the lowest-cost mechanism for building digital products.

The properties of microservices are as transparent as possible to the process of applying new information to a problem.

In place of the craftsmanship approach to building digital products, where fashion, fame, or power reign, the properties of information dictate the processes we use. This provides a basis for measuring and improving efficiency that is independent of particular industries, businesses, and people.

Microservices unify correctness, security, and quality and elevate them to a consistent, inherent aspect of the digital product instead of being an afterthought or add-on.

Most importantly, microservices reverse the trend of technology fueling ever greater centralization and accumulation of power by making collaboration less costly that concentration of control. The rich and varied fabric of humans in society can participate and influence outcomes in a meaningful way.

## Start here

To begin your journey to microservices, here are questions to ask:

1. How do we measure learning?
1. Can we visualize our process?
1. What is our batch size and cycle time?
1. What is the quality of our feedback loops? How do we measure them?
1. What is the cost of our status, testing, and delivery processes?
1. What is the minimum time to deploy any change?
1. What is the smallest change we can deploy?
1. Do we use feature flags to deploy more than one version of a feature?
1. How do we know the system is working after we deploy?
1. Who can suggest a change to our status, testing, or delivery processes?
1. When do we learn about problems in our system?
1. What is the cost of delay when a feature is ready but cannot be delivered?
1. How quickly can we change direction after learning new information?

Now revisit each question. How would your biggest competitor answer them?

---

[^1]: _The High-Velocity Edge_, Steven J. Spear, 2009

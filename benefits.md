# Benefits of a Microservices Platform


## Microservices and the size of a business

The constraints on a business, and the requirements of the principle process of a business, are what make microservices relevant. But what impact will microservices have on the existing business structures?

The economist, R.H. Coase, in his book The Firm, the Market, and the Law says this about the size of a firm (emphasis added):

In my article on "The Nature of the Firm" I argued that, although production could be carried out in a completely decentralized way by means of contracts between individuals, the fact that it costs something to enter into these transactions means that firms will emerge to organize what would otherwise be market transactions whenever their costs were less than the costs of carrying out the transactions through the market. The limit to the size of the firm is set where its cost of organizing a transaction becomes equal to the cost of carrying it out through the market.

This is absolutely fascinating. Let’s see why.

While Coase does not explicitly refer to the firm’s boundary, it is essential to understanding the firm’s size, which is precisely the number of employees inside that boundary.

Consider the boundary of a digital product, like Twitter. Assume that Twitter runs some of its processes on Amazon AWS and some in its own data center.

You open the Twitter application on your phone and start looking at tweets. You notice one that links to an interesting article in The Washington Post. You tap the link and the article is rendered for you. After reading a few paragraphs, you decide to share it with your friend, so you tap the control and select the option to DM your friend the article. Twitter notifies your friend that you’ve shared a DM, and your friend opens their laptop browser to look at your tweet. The friend clicks on the link and visits the main website for The Washington Post, then decides to share the article in an email to a friend.

Where is the boundary of the Twitter digital product, or the boundary of the Twitter app on your phone? Is the interaction itself part of the app, but not the content it renders? Are the AWS instances serving some content to your phone app part of the phone app? What about the servers for The Washington Post?

In a connected world, determining where the boundary of one thing is starts to become extremely difficult.

A recent trend is particularly relevant here, Zero Trust Networks. The idea is simple, there is no longer a privileged boundary (or perimeter) separating "internal" nodes from external ones, and where the internal ones are given a different level of trust than external ones.

That perimeter used to coincide with the boundary of the business, where it controlled the internal nodes but not the external ones. Eliminating that boundary allows rich interactivity, where trust and security are functions of a particular node, not the privileged status due to that boundary.

Businesses have built "APIs" to permit others to use their digital products in a controlled manner, but microservices encourage rich and extensive interactions. Instead of endlessly duplicating functionality, businesses can transparently provide and use highly standardized, or highly customized services.

The leveling of the field for competition that microservices promotes will likely erode the size of firms that we see today.


#### Misunderstanding Value

Code is a liability, not an asset. The code itself should be discarded at the earliest opportunity. The focus of a business should be replicating, transmitting, and refining what it is learning. DNA carries genetic information, but it is the expression of those genes that has value. Similarly, code may be the carrier of the firm's information and learning, but it is the running code that provides value.

testing, pair-wise, contract, collaboration, inductive, isolation property, constant monitoring for correctness, healing and recovery

#### Software Construction Is Not Distributed

Today, any interesting piece of software is talking to other software on a separate physical device. This was not true of most software a few decades ago. That is to say, the boundaries of software are less distinct, and software is inherently distributed.

To illustrate the first point, if this program talks to software that is essential to its functioning, is that software a part of the program?

#### Failure To Exploit Learning

Use of concurrency and approaches to building distributed systems.

#### Poor Adoption Of Technology Advances

The data supporting the use of DevOps to drive favorable business outcomes is well established, but many firms consider adoption to be optional or have not even considered it. Beyond leaving money on the table, this negligence could threaten the existence of many of these businesses.


MVP

standardization, 10,000 times less costly

size of organization

ability to solve real problems, minimum contribution

interoperability

cloud optional, efficiency, trasparency, scaling

security

the idea of whole (coherent) enough to complete a task.

# Trends

## Ubiquitous Computation

## Fragmented Marketplaces

## Platforms

## Minimal Transaction Costs

## Purpose-built

Purpose-built is not the same as customization, it's the opposite of general
purpose.

## De-materialization and De-energization

## Automation of Work


# Rubinius Solutions

## Marketplace

Examples of this are rapidly growing.[^1]

## Model For Building Software

#### Distributed Software Construction By Example

How to build what you want to build.

A recent example of distributed software construction.[^2]

## Technology

#### Instruction Set

Defining computation.

[^3]

#### Language Infrastructure

Supporting language experimentation, innovation, and integration.

#### Mixed Execution

Managed runtime and native code.

#### Memory Models

Open, closed, and isolated.

#### Distributed Code

IPFS

#### Infrastructure

Provide the standard components for distributed software like monitoring, rate limiting, authorization, tracing, and security.

## Business Model

#### Buyers, Sellers and Rubinius

There are three sides to the Rubinius marketplace.

#### Emergent Software

Consistent with the distributed nature of software, the structure itself should emerge from the use of the software.[^4]

#### Knowledge, Skill and Will

Three categories of prospective customers.

#### Beachhead Strategy

Those who want to create something new.

#### Experimenting With Price

Maximizing plans.

#### Driving Fragmentation

Markets can only approach fairness if no participants have unfair influence.

# Opportunities

## Internet of Things

## Augmented Reality

## AI for Knowledge

## Bio-informatics and Health

## Autonomous Vehicles and Robotics


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

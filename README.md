# Code, Compute, Cash

## Reinventing Distributed Software

_Brian Shirai, Rubinius, Inc. April 2018, Version 0.8_

**_Microservices_ are a context-independent and scale-independent architecture for digital products that maximizes applying new information while minimizing its cost.**

Microservices provide a structure for distributed applications that eliminate much of the waste associated with building digital products today because the attributes of microservices align with the unique properties of information.

The primary process of any business is learning, not production, and microservices are an optimal structure for business.

In this paper, we begin in [Part 1](problem.md) with the problem of applying new information to an existing system in a competitive market, and summarize existing procedural and structural flaws that complicate building digital products. Then we define the structure and function of microservices in [Part 2](solution.md). In [Part 3](platform.md) we introduce features of the Rubinius platform that reflect the structure of microservices and aid building them. Finally in [Part 4](benefits.md), we illustrate benefits of microservices relative to the problems of building digital products.

### A note on terminology

Careful use of definitions is essential to precise thinking. Beyond labeling, words provide differentiation. To complicate matters, words acquire their meanings over time. This is critically important in digital products because, as John Day says, _"We build what we measure."_[^1]

There are various definitions of "microservices". While the one presented here may not agree precisely, the intention is that it agree broadly with the spirit of those existing definitions, while perhaps eliminating some aspects that don't appear fundamental and emphasizing others considered essential. Where this definition may vary, we justify that by way of its utility in defining activities that promote the goal of efficiently building digital products. _Microservices are distributed applications, but not all distributed applications are microservices._

### A note on theory

Our purpose is not a _natural history_ of digital architecture. Instead, we desire to understand how information can be applied in a competitive market to successfully build digital products. We seek to understand cause-and-effect and leverage that to gain competitive advantage over our peers. Merely imitating behavior will never provide the leverage we need.

Aspiring to a goal is not the same as attaining the goal. A moment's reflection hopefully convinces us that we should be dissatisfied with anything less than a _theory_ of applying information to build digital products in a competitive market. Whether we are making progress in that endeavor requires the scientific method. We form an explanation.[^2] We make predictions and test them. We extinguish incorrect beliefs[^3] and refine the explanation. Most of what we learn, we could not predict.[^4]

The [web version](https://rubinius.gitbooks.io/whitepaper-code-compute-cash/content/) of this paper permits commenting, which is highly encouraged and appreciated. The paper is also available in PDF, ePub, and Mobi formats [at the GitBook website](https://www.gitbook.com/book/rubinius/whitepaper-code-compute-cash/details).

---

[^1]: _Patterns in Network Architecture_, John Day, Prentice Hall, 2008
[^2]: ["A New Way To Explain Explanation"](https://medium.com/dorothyknows/david-deutsch-a-new-way-to-explain-explanation-e153f981428c)
[^3]: ["Extinction: a Constructor-Theoretic View"](https://medium.com/dorothyknows/chiara-marletto-extinction-a-constructor-theoretic-view-fc567fb02bfc)
[^4]: ["The Unknowable & How To Prepare For It"](https://medium.com/dorothyknows/david-deutsch-the-unknowable-how-to-prepare-for-it-e1b2c7d78744)

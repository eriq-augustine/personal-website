---
layout: page
title: Research
nav-title: Research
order: 4
permalink: /research/
---

In our increasingly connected world, data comes from many different sources, in many different forms, and is noisy, complex, and structured.
To confront modern data, we need to embrace the structure inherent in the data and in the predictions.
An effective means of approaching this problem of structured prediction, is statistical relational learning (SRL).
SRL frameworks use weighted logical and arithmetic expressions to easily create probabilistic graphical models (PGMs) to jointly reason over interdependent data.
However, despite being well suited for modern, interconnected data, SRL has several challenges that keep it from becoming practical and widely used in the machine learning community.
My research addresses four pillars of practicality for SRL systems: scalability, expressivity, model adaptability, and usability.
Much of my work uses and extends [probabilistic soft logic (PSL)](https://psl.linqs.org), an open-source SRL framework that has stood out for its flexibility and ability to efficiently reason over large models.

Scalability in SRL systems allows for the use of large datasets and complex models.
Because of the complex nature of interconnected data, models can easily outgrow memory spaces.
To address scalability for SRL, I build systems that more efficiently and intelligently instantiate PGMs from templates and data [[Augustine MLSys 2018](https://linqs.github.io/linqs-website/publications/#id:augustine-mlsys18)].
I also create fixed-memory inference methods that can perform inference on very large models without requiring a proportional amount of memory [[Srinivasan AAAI 2020](https://linqs.github.io/linqs-website/publications/#id:srinivasan-aaai20b)].
As future work in scalable SRL systems, I have proposed research for scalability that distributes model instantiation across several machines and a system which combines all this work and creates the first SRL system capable of handling models with trillions of connections [[Augustine TPM 2019](https://linqs.github.io/linqs-website/publications/#id:augustine-tpm19)].

Expressivity allows SRL systems to represent many different problems and data patterns.
Because SRL uses logical and arithmetic expressions to represent structured dependencies, SRL frameworks need to be able to express more than just what is represented by feature vectors.
To address expressivity for SRL, I have created a system to incorporate neural models with structured SRL inference, and have expanded the range of PSL hyperparameters to include negative weights [[Dickens TPM 2021](https://linqs.github.io/linqs-website/publications/#id:dickens-tpm21)].
I propose to extend my research for expressivity by expanding the definition of logical operators in PSL to include different types of fuzzy logic such as Gödel logic.

Model adaptability is the ability of SRL frameworks to handle models that change.
A changing model can be as simple as a model that has its hyperparameters tweaked, or as complex as a model that changes its structure over time.
To address model adaptability for SRL, I have created new weight learning approaches for PSL [[Srinivasan MLJ 2021](https://linqs.github.io/linqs-website/publications/#id:srinivasan-mlj21)], and created a system for generalized online inference in PSL [[Dickens ICML 2021](https://linqs.github.io/linqs-website/publications/#id:dickens-icml21)].
My proposed research for model adaptability includes a system that combines both the above techniques into an online weight learning system, and further improving online inference with the ability to forget old and out-dated information.

Usability makes SRL frameworks easy for people to use.
Because of the need to model structural dependencies, SRL frameworks are often harder to use than more common machine learning libraries.
To address usability for SRL, I have created new programming language interfaces to interact with PSL, and a visual model inspector for analyzing and debugging PSL models [[Rodden RecSys 2020](https://linqs.github.io/linqs-website/publications/#id:rodden-recsys20)].
My proposed work for usable SRL systems includes more programming language interfaces to PSL, a general SRL interface spanning multiple SRL frameworks, and a browser-based interactive PSL for users to better see how changes to a model impact the final predictions.

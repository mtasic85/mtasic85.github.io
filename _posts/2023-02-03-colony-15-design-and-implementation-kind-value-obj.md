---
layout: post
title: "Colony #15 - Design and Implementation - kind/value/obj"
date: 2023-02-03 20-09-18
categories: colony
---

I dive deep into the development of the Colony Programming Language, focusing on the implementation of C-level objects (co_obj_t) and other core types. In the beginning, I discuss the key components of the language, such as the object model, syntax, grammar, and parser. I explain the importance of packing these components in a way that minimizes memory usage and maximizes access speed. I also touch on the concept of reference counting, which is a form of garbage collection used in the language. The discussion then moves on to the different types of objects in the language, including bytes, strings, arrays, dictionaries, and functions, among others.

As the video progresses, I delve into the intricacies of the language's structure, discussing the implementation of different types of objects and how they interact with each other. I also explore the concept of context in the language, explaining how it is used when executing functions and importing modules. I emphasize the importance of reducing indirections to simplify the language's implementation and improve its performance.

In the ending of the video, I focus on the concept of 'generic' in the Colony Programming Language. I explain how it can be combined with functions, structs, and unions to create new types. I also discuss the idea of 'generic structs', which are structs that can take another struct and produce a new generic struct. I wrap up the video by discussing the potential for creating native executables from the language's instructions, highlighting the importance of making the integration with code generators as straightforward as possible.

<iframe width="560" height="315" src="https://www.youtube.com/embed/akGmfKo2S_Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
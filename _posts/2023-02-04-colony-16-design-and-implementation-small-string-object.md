---
layout: post
title: "Colony #16 - Design and Implementation - Small String Object"
date: 2023-02-04 17-34-46
categories: colony
---

I explore the complexities of garbage collection, reference counting, and the intriguing concept of immortal objects in the Colony programming language. I kick off the discussion by simplifying the model, removing bytes, and focusing on UTF-8 encoded strings, which are more commonly used by developers. I also introduce the concept of 'small string objects', strings that can fit within 128 bits. The first 64 bits are reserved for the 'kind' of the object, and the remaining 64 bits are used for the string itself. This optimization is particularly applicable to strings because they are immutable by default.

As the video progresses, I delve into the concept of 'immortal objects'. These are objects with a special value of reference count and will have a flag marking them as immortal. Built-in types such as bytes, array, dict, etc., will be marked as immortal as it doesn't make sense to increment and decrement their reference count every time. I also demonstrate how to use these small strings, assuring viewers that the complexities of this implementation will be hidden behind the scenes, making it easier for developers to use.

In conclusion, this video provides a comprehensive overview of the design and implementation of small string objects in Colony. It offers valuable insights into garbage collection, reference counting, and the concept of immortal objects. I believe it's a must-watch for anyone interested in the inner workings of programming languages.


<iframe width="560" height="315" src="https://www.youtube.com/embed/GY-cHUanWEs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
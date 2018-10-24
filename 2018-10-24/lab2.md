# Lab 2

- Date: 2018-10-24
- Session overview: this session is an introduction to Rust. We review several characteristics of other languages and compare Rust to them.

![](https://www.rust-lang.org/logos/rust-logo-blk.svg)

## Notes

### A word on type systems
Learning Rust before Haskell: if you want to learn the functional paradigm, it is recommended that you learn Rust first because of its type system. 

As you know, ```int```, ```char```, etc are types. We can classify languages depending on its typing: static vs dynamic, weak vs strong. C has static weak typing, Javascript has dynamic weak typing, Python has strong dynamic typing. Finally, Haskell and Rust have static and strong typing.

In a Static language, types are determined at compile time. In a Dynamic one, they determined at runtime.

In a Weak system, different types may be comparable (```int a; float b; a < b```, or the Javascript comparison between _any_ two things). This can obviously be dangerous. In a Strongly typed language, most (if not all) type conversions have to be made explicit.

### Rust variables and types
In Rust all variables are defined as ```let var = …```. It has type inference, which assumes the type depending on context. You can also tell it the type you want, for cases in which is absolutely needed or is ambigous.

### Memory management
If we talk about efficiency, any high level language has automatic memory management (via a garbage collector and the like), while Rust (like C and C++) has manual memory management (no gc)

Quote: "I wouldn't step on a plane whose software is running with a garbage collector".

Rust manages memory via its ownership system. When a function ends, it automatically frees all the variables it owns. To make a variable live longer, a function can transfer the ownership to another function when calling it. This system solves the double-free and malloc issues, amongst others.

### Most loved language

Rust is the most loved language in the [stackoverflow 2018 survey](https://insights.stackoverflow.com/survey/2018/#most-loved-dreaded-and-wanted).

--> The rest of the session, we focused on reading through the first resource (*A gentle introduction to Rust*).

## Resources

![](https://stevedonovan.github.io/rust-gentle-intro/PPrustS.png)

- https://stevedonovan.github.io/rust-gentle-intro/
- https://play.rust-lang.org

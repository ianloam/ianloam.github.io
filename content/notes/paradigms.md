---
title: "Nonrepresentational Programming and Multiparadigm Languages"
---
# Nonrepresentational Programming and Multiparadigm Languages
## 1. Background

With Turing Completeness, we develop the idea of whatever is possible in one programming language is also possible in every other. However, this is only true if you narrow your perspective to acknowledge only the formal mathematics of computable functions, while ignoring any broader sense of practical application or language expressiveness. This is instantly clear with esoteric and Turing tarpit languages (such as Brainfuck, Malbolge, etc.) that may have none or limited I/O and abstraction capabilties, among other inconveniences. Implementing an algorithm that may be trivial in C or Python is next to impossible in these languages.

So, how do we measure when a language has not only achieved Turing Completeness, but also some kind of "General Completeness"?

The most evident answer would be by the language's features. Whether it supports certain data-structures, libraries, syntax, garbage collection, type systems, execution models, or any other particular surface aspect of the language implemented to give it structure. If we select a group of features then they can be applied to a defined use-case or problem.

Extending from this, we begin to develop the idea of programming paradigms. Which are families of features that work well toghether and aimed at resembling a specific style of programming (e.g. Imperative, Functional, OOP, etc.).

Thus, when it comes to "General Completeness", it could be achieved through Multiparadigm languages. This is because by implementing a large diversity of programming styles, we accumulate the amount and combinations of features that would potentially hit a targeted use-case.

## 2. Critique of Multiparadigm Languages

While Multiparadigm languages do provide a viable solution to General Completeness, their pursuit of attaining comprehensive features produces a landscape of needless complexity.

/For example, when learning the language for the first time, the user has to deal with an overload of options and frameworks. For some given problem, the user not only has to solve it but navigate through all the features to find the most appropriate approach. This creates another layer of confusion, and needlessly detracts from the labor it took solving that problem.

The paradigms are not always compatible. Features from one paradigm may not integrate seamlessly with those from another, creating edge cases and subtle bugs that can be difficult to diagnose and fix. Even when corrected by the developer, there is always the need for some specialized structure or idiomatic solution (wee see the rise of syntax sugars and conventions like Design Patterns within OOP languages), which in isolation appears convenient, but as they accumulate contribute to an increasingly irregular and unpredictable language.

The design of the language is never finished. Much of the work goes into accomodating new use-cases and for making features across paradigms cohesive, inflating the language and difficulties as time goes on.

Especially when it comes to popular languages with teams of developers, it seems there is a layer of internal politics and bureaucracy required for the continual envisioning of the language. Every decision becomes mediated and subject to petty oversights. 

Overall, despite providing a path toward General Completeness, Multiparadigm languages come with endless strings attached. There is never a point of focus or reliability where you can think about the programming problem on its own./

### 2.1. Design of the C Programming Language

/On the other hand, the design of the C programming language provides an example of this problem independent approach. While not achieving "General Completeness", the design philosophy behind the language avoids the pitfalls of Multiparadigm languages through simplicity and a well-defined scope.

Inspired by the UNIX philosophy, C emphasizes "doing one thing well". For C this is: creating efficient, direct mapping to machine instructions for system-level programming. 
/


## 3. Use-Structures and Programming Paradigms

It seems that between Multiparadigm languages and C we have to choose between General Completeness and problem independence. However, this separation only arises because of our analysis of language design via programming paradigms and features.

We understand that there is a diverse set of applications for programming from web design, low-level systems, etc. with each respective feature to accomodate them. If we were to imagine an expansive map of all features, languages like C would be a small and well established territory while Multiparadigm languages would be growing into every domain.

However, when analyzing this hypothetical map, we begin to see that the territories of features are not as neatly defined as one might think. The boundaries between features tend to blur and overlap. Certain features can be dependent on eachother in unexpected ways, or the same feature can have differing limitations/capabilities depending on the context.

In fact, if we were to ask what is meant by a "feature", we see there could not be a more confused term. Even though we can identify a singular feature at face value, it is far from clear what aspects are just "details" and what is essential for a language's underlying use.

To illustrate, if we were to look at two different languages with the same feature we often observe they mean very different things.

For example, take Lambdas in C++ and Python: in Python (and other interpreted languages) lambdas are executed symbolically by making substitutions to the lambda function directly through the interpreter runtime, but C++ is a compiled language that can not handle symbolic manipulations like this, so lambdas are treated as a black box from a special Functor class which is then compiled and run later from an executable file.

Although the lambdas from both languages ostensibly act the same, the differences in implementation tells us that the mechanism behind what produces the feature's usage comes from a fundamentally different organization and execution process.

We might ask: If they end up being used as the same feature then why do we care about implementation?

The first and obvious answer is that the differences in implementation makes them a different feature, but only in subtle ways. Maybe if we had some problem that asks us to pay close attention to precise details about how lambdas are executed (such as optimization problems or a problem concerning compiler limitations) then we care if the language uses a Functor class or interpreter substitution.

However, more interestingly it 

What different manifestations of more fundamental programming concepts.

More abstractly, 

### 3.1. Primitive Use-Structures

More generally, if we were

### 3.2. Hybrid Compilers
## 4. Nonrepresentational Languages
### 4.1. Design Principles
### 4.2. Key features
### 4.3. Implementation
## 5. Implications and Future Directions
## 6. Conclusion and Final Remarks

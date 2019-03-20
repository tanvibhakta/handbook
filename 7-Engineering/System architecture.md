## System architecture

When dealing with large, complex systems, a key problem is how to evolve the architecture without just throwing everything up in the air and hoping it lands on time. That approach is a thing of the past in our world of continuous engineering and delivery. In fact, even in the past it was problematic since it deferred many of the trickiest and time-consuming integration tasks and was a source of many a late project.

A big challenge of re-architecting a system is recognising subtle inherent (or hidden) requirements since they are often implicit in the way the component is used rather than an explicit part of the API contract.

[Fred Brooks](https://en.wikipedia.org/wiki/Fred_Brooks) differentiates between two different types of complexity: _accidental complexity_ and _essential complexity_. Accidental complexity relates to problems which engineers create and can fix; for example, the details of writing and optimising assembly code or the delays caused by batch processing. Essential complexity is caused by the problem to be solved, and nothing can remove it; if users want a program to do 30 different things, then those 30 things are essential and the program must do those 30 different things.

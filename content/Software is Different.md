Title: Software is Different

Index: software
Index: manufacturing
Index: engineering
Index: architecture
Index: hardware
Index: design
Index: gates
Index: malleability
Index: rework
Index: Humphrey, Watts
Index: Lohr, Steve
Index: Sayre, David
Index: IBM

Body:

When we talk about software development, we often use terms like "engineering" or "architecture," and draw on lessons learned from other environments, implying that developing software is like building a house, or designing a new consumer product.

However, there are some very fundamental differences between software and these other sorts of products, and we need to keep these in mind in order to talk sensibly about software development.

### 1. Triviality of the Manufacturing Step

The goal of software development is to develop something new (to create meaningful variation), while the goal of manufacturing is to build the same thing over and over again (to minimize or eliminate variation).

Within other forms of product development, significant attention is paid to manufacturing the product from a set of design documents. In most cases, many different units will be built of an identical design, so there is a repetitive element to the manufacturing process, resulting in a focus on driving out variation in manufacturing. Also, there is typically a human element in the manufacturing process, and so product quality and the risk of errors introduced in manufacturing receive much attention.

For software, however, the design documents are the program source code, and "manufacturing" consists of building actual executables from the source. This is a process that is completely automated by compilers, linkers and other build tools, and so is relatively trivial.

One implication of this fact is that it is much less meaningful to separate design from construction in software development. In hardware development, it is absolutely essential to create detailed product design models and documents from which physical products can be reliably and repeatedly manufactured. However, since we are only ever building one instance of any detailed software design, there are diminishing returns for increasing levels of detail in software design documentation. And so the software code actually becomes the detailed design documentation.

### 2. Absence of Physical Substance

There is no physical material involved in software construction, so there is no need for material transformation from one form to another, and no need for material transportation from one location to another. In fact, the only thing flowing through the software development process is information. And, unlike material, information can be in two or more places at the same time, and can flow in multiple directions concurrently.

Because there is no need to order raw material or components to feed a physical assembly line, there is no natural "gate" between design and construction, as there is with physical products.

### 3. Product Malleability

Software is easy to change. And once you have changed it, it is easy to regenerate the executables (manufacture it). So while we often talk about the high cost of change, most of the costs are in coordination and communication, and are not fixed costs based on material or manufacturing costs.

And so, while there are rework costs, the "measure twice, cut once" approach is less relevant to software than it is to hardware. And software is often able to evolve more quickly than physical products.

### 4. Diversity of Purpose

While aeronautical engineering, for example, is about making things fly, the purposes to which software can be applied are amazingly diverse, and becoming more so all the time. So the things that work well for someone developing image processing software may be different from what works well for someone developing software to process banking transactions.

### 5. Rapidly Changing Context

When one considers other engineering fields, there is generally some physical context for the discipline that changes infrequently, or not at all. A chemical engineer operates within the field of chemistry, for example, and the number of elements, and the basic chemical laws rarely if ever change. Other engineering fields are based on physics, or thermodynamics, or some other relatively unchanging body of knowledge about the physical world.

On the other hand, software "engineers" are operating within the constraints of the hardware available to them, and within the specified software environment -- both of which are changing rapidly, and often in unpredictable ways.

So if a student studies chemical engineering, then he or she can be relatively confident that what they learn will be of use to them over their entire careers as chemical engineers.

On the other hand, software engineers often study languages, operating systems and hardware environments that may be entirely different five years after they have completed their studies.

### 6. Layers of Abstraction

Related issues are the complexity and mutability of the layers of software abstraction surrounding the problem domain in which the software developer is working.

Many developers today, for example, develop software that sits on top of an operating system, a database management system, application integration middleware, a web server, an application server and a set of language subroutine/class libraries, all of which are in more or less constant flux.

### 7. Scale

Watts Humphrey has made the point that a civil engineer, when considering the height of a structure, only has to worry about roughly two orders of magnitude difference between the smallest and the largest product he is likely to be called upon to design: that is, the tallest structure he is likely to work on is no more than roughly 100 times the size of the shortest structure.

On the other hand, software developers in college start out learning to write individual programs of roughly 1000 lines -- but then, in the real world, are expected to work on projects developing more than a million lines of code: in other words, a difference of roughly three orders of magnitude.

Humphrey has gone on to suggest strongly that practices that work well at the lower end of this range are not likely to scale well to the upper end.

----

<blockquote>
<p>
The desire to treat software more like its hardware siblings began in earnest in the 1960s. Equal treatment was one motivation, at least at the start, but it was also an effort to make programming a more structured discipline like hardware engineering. Looking back, [David] Sayre observed that the Bald Peak conference had the regrettable effect of beginning a management mentality that served to &#8220;rigidify&#8221; programming at IBM. In the early days, he recalled that programming at IBM had an informal Silicon Valley flavor, which tended to encourage innovation. By the late 1960s, the working environment had become much more regimented. The disciplines of hardware engineering fit uneasily in the more ethereal realm of software. &#8220;Software is a much more plastic object than hardware,&#8221; Sayre said. &#8220;You whip it up, squeeze it, and you can dream.&#8221;</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Steve_Lohr">Steve Lohr</a> from the book <cite><a href="bibliography.html#lohr-2002">Go To</a></cite> Copyright &copy; 2001 by Steve Lohr
</p>
</blockquote>

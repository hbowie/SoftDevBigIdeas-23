Title: Just Enough Design Up Front

Index: BDUF
Index: Case Western Reserve University
Index: Constantine, Larry
Index: Gall, John
Index: Gehry, Frank
Index: JEDUF
Index: Lockwood, Lucy
Index: Poppendieck, Mary and Tom
Index: Reeves, Jack W.
Index: YAGNI (https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)
Index: architectural runway
Index: architecture
Index: code as design
Index: cowboy development
Index: design
Index: refactoring (https://en.wikipedia.org/wiki/Code_refactoring)


Body:

When addressing the question of how much design should be completed before coding starts, there are several factors to consider.

1. Design changes are generally harder and more expensive to make after software code has been written.

2. Architects and designers are sometimes better qualified to perform design than other team members, and it is easier to confine design tasks to these few individuals before more developers get involved.

3. Some overarching design decisions need to be made in order to enable more detailed work to proceed.

4. The wisdom of a design can only be fully validated once it is implemented in working software.

5. Work done later in the effort can draw upon the skills, experience and wisdom available from the larger [team][teams].

6. The team will learn more about the problem space as the work progresses, and so deferred design decisions can take advantage of these greater learnings.

7. Early design decisions often turn out to have been based on mistaken assumptions, or on evolving business conditions that then change before the software is ready for delivery and use.

8. When design is done early, there is a tendency to provision for features that later turn out to be unneeded. This is one reason why agile practitioners try to follow the "[YAGNI][]" dictum: until proven otherwise, assume that "You Ain't Gonna Need It".

9. Developers will be more fully [engaged][engagement] in the work if they are focused on the overall purpose of the effort, and are allowed sufficient autonomy to make some design decisions as they work.

10. If designs become large and complex before any of their elements have been validated by working code, then the number of invalid elements embedded in the design may be too numerous and widespread to allow the resulting system to ever function correctly. 

If we consider only the first three factors, then we will do all of our design work using models and documents before writing a single line of code. This is sometimes referred to as Big Design Up Front (BDUF).

If we consider only the last seven factors, then we may be tempted to rely entirely upon emergent design, without any up-front architecture. This is often referred to as "cowboy development," since we are always shooting from the hip, without ever stopping to take careful aim at our target.

When we take all of these considerations into account, though, we generally find it best to do some early design work, but allow the full design to emerge as the work progresses.

This is why it is usually best to practice JEDUF: Just Enough Design Up Front.

The advantages of such an approach are not confined to software development. Here is an example of how Frank Gehry and his team designed and built the Peter B. Lewis Building at Case Western Reserve University, as described in <cite>[A Perfect Mess: The Hidden Benefits of Disorder][abrahamson-freeman-2006]</cite>, by Abrahamson and Freeman:.

> The school approved the design and brought in a small army of contractors to build it. The contractors duly admired, in a shocked and fretful way, the model of the God-awfully complex structure they were about to undertake, and then asked for the blueprints, to which Gehry's team replied that there weren't any.
>
> To capture the building's emotional content, Gehry maintains, everyone working on the building should keep creating throughout the construction process.
>
> Freed from the constraints of a blueprint's rigid specifications… the contractors and architects were able to collaboratively rethink the design and construction techniques in any way necessary to achieve the project's goals. That led to an eruption of innovation.
>
> Not only was the finished building a stunning hit, completed on time and within budget, but most of the contractors were so pleased with the invention into which they had been pushed that they ended up changing the way they do business.

Early stages of design are often referred to as architecture.  When we discuss the architecture of a system, there are at least five different (albeit related) areas that must be considered.

* Information: What are the major entities/objects/facets to be considered by the system, and how will each of these things be identified?

* Functional: What business functions will be performed, and how do they relate to each other, and to other functions that are out of scope?

* User Interface: How will the user navigate through the system, what will the system look like, and what sort of special controls or other UI elements may be needed?

* Technology/Infrastructure: What are the technologies to be used by the project, and what roles will those technologies play? On what infrastructure (both hardware and software) will the application run? What development tools will be used?

* Software: What software modules, or types of modules, will be written, and how will they relate to each other?

Note that, even with some upfront architecture, development teams may still need to schedule some periods of concentrated architectural work later in the project. This is sometimes referred to as extending the architectural runway, with the idea that the architecture is necessary to support the user functionality, and so as the functional development proceeds, it gets closer to the end of the existing runway, necessitating the dedication of resources to further building out the architecture in order to allow the continued functional work to proceed smoothly.

For additional details on this topic, see the Pagan Tuna post, &ldquo;<a href="http://www.pagantuna.com/posts/agile-architecture.html" class="reflink" target="ref">Agile Architecture</a>.&rdquo;

----

<blockquote>
<p>
We need to adopt the attitude that the internal structure of a system will require continuous improvement as the system evolves. Refactoring &#8212; improving the design as the system develops &#8212; is not just for commercial software. Without continuous improvement, any software system will suffer. Internal structures will become calcified and fragile. In a surprisingly short time, the system will cease to be useful.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Mary_Poppendieck">Mary Poppendieck</a> and <a href="http://en.wikipedia.org/wiki/Tom_Poppendieck">Tom Poppendieck</a> from the book <cite><a href="bibliography.html#poppendieck-2003">Lean Software Development: An Agile Toolkit</a></cite>
</p>
</blockquote>

----

<blockquote>
<p>
Prototypes and prototyping are not substitutes for analysis and design, not excuses for sloppy thinking.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Larry_Constantine">Larry Constantine</a> and <a href="http://en.wikipedia.org/wiki/Lucy_Lockwood">Lucy Lockwood</a> from the book <cite><a href="http://www.amazon.com/exec/obidos/ASIN/0201924781/pagantuna-20">Software for Use: A Practical Guide to the Models and Methods of Usage-Centered Design</a></cite> Copyright &copy; 1999 by the ACM Press
</p>
</blockquote>

----

<blockquote>
<p>A complex system that works is invariably found to have evolved from a simple system that worked. The inverse proposition also appears to be true. A complex system designed from scratch never works and cannot be patched up to make it work. You have to start over beginning with a working simple system. </p>

<p class="bq-footer">
<a href="https://en.wikipedia.org/wiki/John_Gall_(author)">John Gall</a> from the book <cite><a href="bibliography.html#gall-1975">Systemantics: How Systems Work and Especially How They Fail</a></cite> Copyright &copy; 1975 by John Gall
</p>
</blockquote>

----

<blockquote>
<p>
The final goal of any engineering activity is some type of documentation. When a design effort is complete, the design documentation is turned over to the manufacturing team. This is a completely different group with completely different skills from the design team. If the design documents truly represent a complete design, the manufacturing team can proceed to build the product. In fact, they can proceed to build lots of the product, all without any further intervention of the designers. After reviewing the software development life cycle as I understood it, I concluded that the only software documentation that actually seems to satisfy the criteria of an engineering design is the source code listings.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Jack_W._Reeves">Jack W. Reeves</a> from the essay <cite><a href="bibliography.html#reeves-1992">Code as Design</a></cite>, &#8221;What is Software Design?&#8221; Copyright &copy; Fall 1992 by Jack W. Reeves
</p>
</blockquote>

[engagement]: increase-developer-engagement.html

[teams]: build-great-teams.html

[yagni]: https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it

[abrahamson-freeman-2006]: bibliography.html#abrahamson-freeman-2006

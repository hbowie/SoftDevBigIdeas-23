Title:  Just Enough Design Up Front

Seq:    5.10

Idea Number: 37

Level:  3 - Article

Class:  idea

Timestamp: 20160606174015

Index:  BDUF; Case Western Reserve University; Constantine, Larry; Gall, John; Gehry, Frank; JEDUF; Lockwood, Lucy; Poppendieck, Mary and Tom; Reeves, Jack W.; YAGNI (https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it); architectural runway; architecture; code as design; cowboy development; design; refactoring (https://en.wikipedia.org/wiki/Code_refactoring); 

Body:

When addressing the question of how much design should be completed before coding starts, there are several factors to consider.

1. Design changes are generally harder and more expensive to make after software code has been written.

2. Architects and designers are sometimes better qualified to perform design than other team members, and it is easier to confine design tasks to these few individuals before more developers get involved.

3. Some overarching design decisions need to be made in order to enable more detailed work to proceed.

4. The wisdom of a design can only be fully validated once it is implemented in working software.

5. Work done later in the effort can draw upon the skills, experience and wisdom available from the larger [[Build Great Teams|team]].

6. The team will learn more about the problem space as the work progresses, and so deferred design decisions can take advantage of these greater learnings.

7. Early design decisions often turn out to have been based on mistaken assumptions, or on evolving business conditions that then change before the software is ready for delivery and use.

8. When design is done early, there is a tendency to provision for features that later turn out to be unneeded. This is one reason why agile practitioners try to follow the "[YAGNI][]" dictum: until proven otherwise, assume that "You Ain't Gonna Need It".

9. Developers will be more fully [[Increase Developer Engagement|engaged]] in the work if they are focused on the overall purpose of the effort, and are allowed sufficient autonomy to make some design decisions as they work.

10. If designs become large and complex before any of their elements have been validated by working code, then the number of invalid elements embedded in the design may be too numerous and widespread to allow the resulting system to ever function correctly. 

If we consider only the first three factors, then we will do all of our design work using models and documents before writing a single line of code. This is sometimes referred to as Big Design Up Front (BDUF).

If we consider only the last seven factors, then we may be tempted to rely entirely upon emergent design, without any up-front architecture. This is often referred to as "cowboy development," since we are always shooting from the hip, without ever stopping to take careful aim at our target.

When we take all of these considerations into account, though, we generally find it best to do some early design work, but allow the full design to emerge as the work progresses.

This is why it is usually best to practice JEDUF: Just Enough Design Up Front.

The advantages of such an approach are not confined to software development. Here is an example of how Frank Gehry and his team designed and built the Peter B. Lewis Building at Case Western Reserve University, as described in <cite>[[A Perfect Mess: The Hidden Benefits of Disorder]]</cite>, by [[Eric Abrahamson and David H. Freeman]]:

{:include-quote-body:Building without blueprints}

Early stages of design are often referred to as architecture.  When we discuss the architecture of a system, there are at least five different (albeit related) areas that must be considered.

* Information: What are the major entities/objects/facets to be considered by the system, and how will each of these things be identified?

* Functional: What business functions will be performed, and how do they relate to each other, and to other functions that are out of scope?

* User Interface: How will the user navigate through the system, what will the system look like, and what sort of special controls or other UI elements may be needed?

* Technology/Infrastructure: What are the technologies to be used by the project, and what roles will those technologies play? On what infrastructure (both hardware and software) will the application run? What development tools will be used?

* Software: What software modules, or types of modules, will be written, and how will they relate to each other?

Note that, even with some upfront architecture, development teams may still need to schedule some periods of concentrated architectural work later in the project. This is sometimes referred to as extending the architectural runway, with the idea that the architecture is necessary to support the user functionality, and so as the functional development proceeds, it gets closer to the end of the existing runway, necessitating the dedication of resources to further building out the architecture in order to allow the continued functional work to proceed smoothly.

For additional details on this topic, see the Pagan Tuna post, &#8220;[[Agile Architecture]].&#8221;

----

##### Words from Others on this Topic

{:include-quote:Refactoring as continuous improvement}

{:include-quote:No substitutes for analysis and design}

{:include-quote:Start with a working simple system}

{:include-quote:Source code as design}

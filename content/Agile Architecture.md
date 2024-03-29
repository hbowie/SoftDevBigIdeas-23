Title:  Agile Architecture

Tags:   Agile

Seq:    8.1

Level:  3 - Article

Class:  section

Timestamp: 20230220242053

Body:

*Originally published at PaganTuna.com on 31 Jan 2016.*

Many [Agilistas][] view any discussion of architecture as the first step down a slippery slope that, once taken, will inevitably lead a project into the fiery pit of waterfall.

Let's see if we can unpack this subject a bit, and possibly even reach agreement on a sensible way to do architecture on agile software development projects, especially large and complex ones.

<h2 id="table-of-contents">Table of Contents</h2>

<div id="toc">
<ul>
  <li>
    <a href="#architecture-vs-design">Architecture vs. Design</a>
  </li>
  <li>
    <a href="#architectural-areas">Architectural Areas</a>
  </li>
  <li>
   <a href="#architectural-drivers">Architectural Drivers</a>
  </li>
  <li>
    <a href="#consideration-of-alternatives-and-tradeoffs">Consideration of Alternatives and Trade-Offs</a>
  </li>
  <li>
    <a href="#timing-of-architecture-and-design">Timing of Architecture and Design</a>
  </li>
  <li>
    <a href="#architectural-runway-and-enabler-epics">Architectural Runway and Enabler Epics</a>
  </li>
  <li>
    <a href="#a-project-roadmap">A Project Roadmap</a>
  </li>
  <li>
    <a href="#architectural-deliverables">Architectural Deliverables</a>
  </li>
  <li>
    <a href="#project-cadence">Project Cadence</a>
  </li>
  <li>
    <a href="#design-reviews-and-gates">Design Reviews and Gates</a>
  </li>
  <li>
    <a href="#what-about-detailed-design">What About Detailed Design?</a>
  </li>
  <li>
    <a href="#what-about-emergent-learning">What About Emergent Learning?</a>
  </li>
  <li>
    <a href="#who-does-architecture">Who Does Architecture?</a>
  </li>
</ul>
</div>


First of all, what do we mean by architecture?

There are at least two different points to be clarified here.


<h2 id="architecture-vs-design">Architecture vs. Design</h2>

The terms architecture and design have very similar definitions, so in many contexts they are used to denote the same thing, and are used interchangeably.

If we are to try to make a distinction, though, then architecture usually refers to a more elevated level of design, expressed at a higher level of abstraction, and/or an earlier stage of design.

More significantly perhaps, architecture may prescribe a series of patterns to be used on the project, with instantiation of those patterns constituting more detailed design work.

In this sense, the overall solution architecture must be established before detailed design can occur, and the detailed design must work within, and be constrained by, the overall architecture.


<h2 id="architectural-areas">Architectural Areas</h2>

When we discuss the architecture of a system, there are at least five different (albeit related) areas that must be considered.

* Information: What are the major entities/objects/facets to be considered by the system, and how will each of these things be identified?

* Functional: What business functions will be performed, and how do they relate to each other, and to other functions that are out of scope?

* User Interface: How will the user navigate through the system, what will the system look like, and what sort of special controls or other UI elements may be needed?

* Technology/Infrastructure: What are the technologies to be used by the project, and what roles will those technologies play? On what infrastructure (both hardware and software) will the application run? What development tools will be used?

* Software: What software modules, or module types, will be written, and how will they relate to each other?

If you are missing any one of these, then you don't have a complete architecture.


<h2 id="architectural-drivers">Architectural Drivers</h2>

Architecture is driven primarily by four different items.

* Enterprise Architecture: The application architecture must work within Enterprise standards, principles and guidelines.

* Segment/Domain Architecture: Similarly, the application must respect the boundaries and guidance established for the particular domain that it occupies.

* Business/Functional Requirements: The application architecture will obviously be strongly influenced by the particular business functions the application must perform.

* Non-Functional Requirements (NFRs): These are often requirements that define desired quality attributes of the system to be developed.


<h2 id="consideration-of-alternatives-and-tradeoffs">Consideration of Alternatives and Trade-Offs</h2>

Whether you are using agile practices or a more traditional methodology, one hallmark of a worthwhile approach to architecture/design is the consideration of alternatives, and the evaluation of trade-offs between those alternatives.

A common error is to assume certain architectural elements and so to adopt them without discussion, perhaps because developers on the team have used certain architectures before, and so bring them along with them to their next project.

In this respect, it is helpful to keep in mind some [research on diversity][forbes] indicating that more heterogenous teams often feel that they are struggling and floundering when compared to more homogenous ones, and yet actually perform better than their less diverse counterparts.


<h2 id="timing-of-architecture-and-design">Timing of Architecture and Design</h2>

In traditional software development, architecture and design are typically done and completed before coding starts, as part of the well known [waterfall approach][wf].

Some agile enthusiasts advocate for the opposite approach, touting "[emergent design][emdesign]," and simply jump into coding with little or no architectural preparation. And while this may work for small efforts building on established architectures, it often falls short in larger efforts, and may lead to floundering and rework and poor designs that fail to stand up over time.

A reasonable compromise is represented by the "JEDUF" approach: Just Enough Design Up Front. With this approach some major design decisions are made before coding, while still allowing for more detailed design to emerge during development, and with the understanding that some refactoring may occur, in order to optimize designs in the face of new discoveries that will arise along the way.

On large projects/programs, however, the combination of some initial architecture, followed by emergent design during sprints, may still not be sufficient to provide for the right amount of architecture at the right time.


<h2 id="architectural-runway-and-enabler-epics">Architectural Runway and Enabler Epics</h2>

When decomposing the work to be done on a large agile project, it can be useful to start with a number of epics to be implemented, with each epic later being broken down into a number of features, and each feature eventually being broken down into stories.

With this approach, it may be helpful to distinguish between Architectural epics and Business/Functional epics, with the former laying the foundation upon which the latter will be built.

Another popular way to think about this is that the Architectural epics extend the runway far enough to allow the Business/Functional epics to proceed without disruption, with the architecture always being done just far enough in advance to prevent the business/functional work from running out of runway.

The [Scaled Agile Framework][safe] (SAFe) calls these architectural pieces of work "[enablers][]," and that's a good way to think about them: the enablers allow the next chunk of business/functional development to proceed.


<h2 id="a-project-roadmap">A Project Roadmap</h2>

Agile projects try to maximize flexibility by lumping all work to be done into a backlog, with the idea that items can be added, subtracted and reprioritized at will, without any unnecessary constraints on content or sequence of execution.

While this sort of flexibility is admirable, by the time you are building a high level backlog out of both enabler and business epics, your are certainly beginning to run into some dependencies that will suggest some sequence to the work to be done.

At this point, it is probably best to begin to represent the epics to be worked -- both enablers and business epics -- in a roadmap of some kind, and not simply as a backlog.

The roadmap should still be subject to change -- it shouldn't be cast in stone -- but it is important to understand when various pieces of runway will need to be extended, and what other work will need that runway in order to proceed.


<h2 id="architectural-deliverables">Architectural Deliverables</h2>

Agile practitioners are sometimes a bit vague about what is actually produced out of architectural work, and so it is worthwhile to be explicit about what deliverables will be produced by enabler epics. These deliverables essentially fall into three categories.

* Reference designs, including patterns, to be used by subsequent business/functional development.

* Hardware and software components (infrastructure and/or reusable application components) needed to enable later business/functional work. These are not just designs, but actual bits of hardware and software that can be used by the application.

* Proofs of concept that demonstrate the feasibility of the design work done, and the readiness to proceed with subsequent business/functional development.


<h2 id="project-cadence">Project Cadence</h2>

A foundational element of all agile development is the regular cadence of the work being done. Teams work in short sprints (aka iterations) of 1 - 4 weeks. More substantial projects may group multiple team sprints into larger chunks of work, such as the "[Program Increments][pi]" (or PIs) defined by SAFe. The work to be done is then subdivided into pieces small enough that they can be worked reliably within this regular cadence, rather than adjusting start and stop dates to fit the size of the work.

But how do we fit architectural work into such a cadence?

If any accommodation for this work is made at all, it is sometimes done by allowing for some fixed amount of architecture work to be done at the start of each iteration, or each program increment, or at the end of each, in preparation for the next.

There are two problems with this sort of cadenced approach to architecture:

* The need for architectural work does not occur at such regular intervals;

* The length of time needed for each piece of architecture can vary considerably, and so cannot be reliably squeezed into a fixed amount of time for each increment.

A better approach is to allow the work planned for each iteration/increment to consist of some combination of architectural enablers and business/functional development, with the amount of architectural work and its timing determined based on the project roadmap being followed.

An enabler epic, then, could be started at any point in the project, and could complete after one, two or three or more iterations/increments -- as many as are needed to complete the work.

These intermittent injections of architectural work into the team's regular cadence are sometimes referred to as "spikes," a term that reflects the uneven distribution of this work over the course of the project.

With such an approach, once the pump is primed with the initial architecture, enabler work and business development will proceed in parallel, with the enabler work timed to keep the runway built in advance of the proceeding business work.


<h2 id="design-reviews-and-gates">Design Reviews and Gates</h2>

If you are working in an environment where design reviews and perhaps even firm gates are required, then the natural place for these to occur is at the end of each architecture/enabler epic. These can be planned in advance based on the project roadmap, and the deliverables specified above can be inspected as part of these reviews.


<h2 id="what-about-detailed-design">What About Detailed Design?</h2>

The detailed functional design of particular screens, reports and interfaces can be done as part of the normal development work done within each iteration/increment, so long as this work is based on the more general architectural work already performed.


<h2 id="what-about-emergent-learning">What About Emergent Learning?</h2>

The guidance provided above is intended to help large and complex projects navigate their ways through some of the difficulties often encountered when doing architectural work.

But the desire to rigidly follow an established architecture must always be weighed against the potential benefits of adapting to take advantage of new learnings that emerge doing the development work.

It is always good to design before you build, but software development is a complex business, and there is no guarantee you will get everything right before you start building.


<h2 id="who-does-architecture">Who Does Architecture?</h2>

In a large enterprise, you will often have several layers of architects.

Enterprise architects sit at the top of the pyramid, helping to guide and govern development work across the entire scope of the business, and establishing principles and standards to be followed by projects.

At the next layer, you may have domain/segment architects, who try to understand a particular segment of the business, and work out the relationships between the various data stores and applications serving that domain.

Application architects, then, will be responsible for the architecture of particular applications, and it is this work that has been the focus of our discussion today.

Within agile, the explicit role of an architect is often omitted, giving way to the egalitarian desire to let all developers participate equally in design work. And while it is generally good to foster creativity throughout the team, and to empower developers to contribute to design work, the truth is that in most successful agile projects you will find a lead developer who ends up guiding and shaping most of the architecture/design for the application. You can call him or her what you will, but once you set out to be more intentional about the way architecture/design work is performed on an agile project, you will also need to be a bit more explicit about the roles involved as well.


[agilistas]: http://www.urbandictionary.com/define.php?term=Agilista
[emdesign]: http://www.agilesherpa.org/agile_coach/engineering_practices/emergent_design/

[enablers]: http://scaledagileframework.com/agile-architecture/

[forbes]:   http://www.forbes.com/2009/06/02/diversity-collaboration-teams-leadership-managing-creativity.html

[pi]:       http://scaledagileframework.com/program-increment/

[safe]:     http://scaledagileframework.com/

[wf]:       https://en.wikipedia.org/wiki/Waterfall_model

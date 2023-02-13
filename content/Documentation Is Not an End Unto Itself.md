Title: Documentation Is Not an End Unto Itself

Index: documentation
Index: Victorian Novel
Index: wikis
Index: Javadoc
Index: approvals
Index: change management
Index: version control
Index: zombies
Index: DeMarco, Tom

Body:

The following forms of waste are all frequently associated with software documentation:

* Documents that are too long and dense for anyone to actually read;

* Documentation that is too vague, imprecise or poorly written to be useful;

* Documents that might be useful, if only one could find them when they were needed;

* Documentation that is not kept up-to-date, and so can be useless at best, and actively misleading at worst.

Concise, well-written documentation can be useful, but one must remember that it is only a means to an end, and one must avoid the various common forms of waste listed above.

Consider alternatives to the traditional Victorian Novel style of project documents. Modeling tools, databases, spreadsheets, diagrams, <a href="https://en.wikipedia.org/wiki/Wiki" class="reflink" target="ref">wikis</a>, and systematically formatted comments (such as those produced by <a href="https://en.wikipedia.org/wiki/Javadoc" class="reflink" target="ref">Javadoc</a>) all often offer better forms of documentation.

Watch out for those who tend to [polarize][balance] this discussion into 'document everything' vs. 'document nothing,' since both of those extremes are generally disastrous. Also watch out for ceremonial approvals of documents: When ten people have to approve everything that's been written down, that's a sure sign that no one understands any of it and no one trusts anyone else.

The first step on the road to documentation sanity is to ask ourselves whether we have a good reason for creating a document.

## Reasons for Documentation

There are generally three different reasons to create software documentation. These three broad purposes really correspond to three distinct audiences. All software documentation should be aligned with one (or, ideally, more) of these three purposes.

These three purposes are:

A. To clarify expectations among those involved in the project;

B. To define and explain aspects of the system useful to future users and developers, and not readily apparent from examination of the software itself;

C. To provide transparency of agency and intention to potentially interested parties outside of the project.

## Elaboration on Reasons

Now that you've seen the list in its entirety, let me elaborate with some additional comments and corollaries.

### A. To clarify expectations among those involved in the project.

1. By "those involved in the project," I mean to include people and organizations involved in the project to any degree, including customers, sponsors, architects, etc.

2. By "clarify expectations," I mean to imply that written documentation will not necessarily be the only, or even the primary, communications vehicle used to establish those expectations.

3. An important corollary is that, if expectations are already clear, or can be more readily clarified through some other, more effective or cost-efficient form of communication, then the software documentation is not needed.

4. Another important corollary is that, if the documentation does not actually provide any clarity, then it's not fulfilling its purpose.

5. Note that expectations can become muddied over time, due to memory lapses, or competition with other information, so part of this clarification of expectations may actually be as a reminder of what had been clear at one time in the past.

### B. To define and explain aspects of the system useful to future users and developers, and not readily apparent from examination of the software itself.

1. Some level of system documentation typically needs to be done to help clarify aspects of the system over what is often a fairly long useful life for the software we write.

2. Both users and developers tend to develop their knowledge of a system through examination of the software itself: users, through the user interface and actual behavior of the software, and developers, additionally, through the examination of the source code. This is often the case because the actual software is typically more credible and as easy or easier to understand than the documentation.

### C. To provide transparency of agency and intention to potentially interested parties outside of the project.

1. This is often the purpose that is hardest for developers to understand and accept.

2. In cases where software produces inaccurate or even dangerous results, outside parties often need access to documentation that will indicate who authorized the offending code, and with what intent.

3. Even if such problems seem unlikely (as they often do, to people closest to the software), such transparency can be justified to help deter malicious or careless software changes.

4. A critical aspect of this sort of documentation is that it be part of an unbroken chain starting with a real request from a real person, and ending with the actual lines of software code that were changed.

## Guidance

OK, now that we're clear on the purpose of our documentation, how does this help?

I believe there is some very practical guidance we can provide, based on the purpose of the documentation.

### If the purpose of your documentation is to clarify expectations among those involved in the project, then:

1. Be aware that the need for such documentation (although not its effectiveness) seems to increase exponentially with the size of the project, both in terms of team size and duration. The smaller the project, the less of this sort of documentation you will need.

2. If you are stuck with a large project, then [decomposing][decomposition] it into smaller sub-projects that can be done in parallel and/or serially can help to reduce the amount of documentation needed.

3. On large projects, plan for the necessary resources to do a good job of the documentation, with enough time and the right resources to produce documentation that team members will actually find useful. Remember that, all other things being equal, more documentation is worse, and concise, easily understood documentation that focuses on the most likely issues of confusion/contention is better.

### If the purpose of your documentation is to define and explain aspects of the system useful to future users and developers, and not readily apparent from examination of the software itself, then:

1. Detailed developer documentation is best maintained within the source code itself. Since developers will look at the code anyway, your documentation is much more likely to be read and maintained if it is included as comments within the program code.

2. High level documentation should be sparse enough that it has a reasonable chance of being read and maintained over the life of the system. Focus on high-level information, like design intent, that is often hard to abstract from the code itself.

3. If your users are having a hard time understanding your system, then your time may be better spent on improving the user interface than on additional documentation (that many will likely not read anyway).

### If the purpose of your documentation is to provide transparency of agency and intention to potentially interested parties outside of the project, then:

1. The larger the project, the more tangled these issues become so, again, shorter and smaller projects tend to require less documentation.

2. The best way to accomplish the needed traceability is through automated change management and version control systems that are joined at the hip, with both the source code itself and the system documentation being under version control.

----

<blockquote>
<p>
When you find a project team that is focused on producing a standard document rather than on considering the content of that document, then you are in the land of the template zombies.... </p>

<p>
In the land of the template zombies, form takes precedence. It is not necessary to think about the content of the document. It is not really necessary to think at all. The important thing is to have something&#8212;anything&#8212;under each of the prescribed headings. Not surprisingly, template zombies are adept in the art of cutting and pasting and ignoring anything that does not fit the dictates of the template.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Tom_DeMarco">Tom DeMarco</a>, <a href="http://en.wikipedia.org/wiki/Peter_Hruschka">Peter Hruschka</a>, <a href="http://en.wikipedia.org/wiki/Tim_Lister">Tim Lister</a>, <a href="http://en.wikipedia.org/wiki/Steve_McMenamin">Steve McMenamin</a>, <a href="http://en.wikipedia.org/wiki/James_Robertson">James Robertson</a> and <a href="http://en.wikipedia.org/wiki/Suzanne_Robertson">Suzanne Robertson</a> from the book <cite><a href="bibliography.html#demarco-et-al-2008">Adrenaline Junkies and Template Zombies: Understanding Patterns of Project Behavior</a></cite> Copyright &copy; 2008 by Authors
</p>
</blockquote>

----

<blockquote>
<p>
If you keep probing, and ask &#8216;Precisely what is in the document? What is it for? Who uses it to make which decisions?&#8217; then you discover that people do not know why. They are producing the document because it is the next thing to do. </p>

<p>
If you recognize this behavior on your project, you may be working in a paper mill. </p>

<p>
In a paper mill, every activity is marked by the production of a document, and progress is measured by how many of the documents have been produced&#8212;not by what the documents contain. The paper mill principle says: Just in case anyone needs anything, let&#8217;s give everbody everything.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Tom_DeMarco">Tom DeMarco</a>, <a href="http://en.wikipedia.org/wiki/Peter_Hruschka">Peter Hruschka</a>, <a href="http://en.wikipedia.org/wiki/Tim_Lister">Tim Lister</a>, <a href="http://en.wikipedia.org/wiki/Steve_McMenamin">Steve McMenamin</a>, <a href="http://en.wikipedia.org/wiki/James_Robertson">James Robertson</a> and <a href="http://en.wikipedia.org/wiki/Suzanne_Robertson">Suzanne Robertson</a> from the book <cite><a href="bibliography.html#demarco-et-al-2008">Adrenaline Junkies and Template Zombies: Understanding Patterns of Project Behavior</a></cite> Copyright &copy; 2008 by Authors
</p>
</blockquote>

[balance]: software-development-is-a-balancing-act.html
[decomposition]: decomposition.html

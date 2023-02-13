Title:  Quality Requires Extra Effort

AKA:    quality

Level:  1 - Book

Timestamp: 20160614153509

Index:  quality; Non-Functional Requirement; NFR; Gawande, Atul; checklists; Humphrey, Watts; ilities; surgeons; Deming, W. Edwards; Glass, Robert L.; Cost of Quality (http://en.wikipedia.org/wiki/Quality_costs); CoQ (http://en.wikipedia.org/wiki/Quality_costs); inspections; peer reviews; pair programming; Kim, Gene; Behr, Kevin; Spafford, George; 

Body:

Most software developers enjoy programming. And most developers enjoy pleasing their customers. This means that, left to their own devices, developers will tend to focus on quickly delivering new features to their customers.

The problem here is that some attributes of high-quality software are not immediately visible to customers. And so, left to their own devices, many developers will tend to give short shrift to these quality factors.

Of course it is human nature to pay more attention to short-term consequences than long-term ones. The fact that the cookie tastes good today sways us more than the fact that it will add to our growing waistline tomorrow. And the chain of causality linking our actions today to long-term consequences often seems murky, further decreasing the likelihood that we will take the necessary actions today to achieve our desired ends. And then there are the all-too-common budget and schedule and content pressures that further coerce developer attention onto these short-term, highly visible results.

Much of the benefit of Agile arguably comes from moving many of these consequences from the long-term to the short-term: continuous integration, for example, means that the build is broken today, not at some far distant point in the future when integration happens.

Some might argue that Agile effectively moves *all* significant consequences into the short term, but I don't believe this to be the case. Some quality attributes tend not to be as readily apparent as other software attributes, no matter how many agile practices you implement.

Following is a list of some of the most commonly identified software quality attributes. These are sometimes referred to collectively as the "ilities," based on the way most of these terms end.

* Accessibility
* Availability
* Compliance with Standards
* Continuity
* Correctness of Results, even under extreme or unusual or novel conditions
* Extensibility
* Graceful Failure
* Maintainability
* Manageability
* Operability
* Portability
* Recoverability
* Reliability
* Scalability
* Security
* Stability
* Survivability
* Testability
* Usability

Since developers often have little natural motivation to focus on these attributes, a project must generally exert some extra effort to ensure adequate levels of quality.

Such extra effort could include any or all of the following:

* <a href="https://en.wikipedia.org/wiki/Non-functional_requirement" class="reflink" target="ref">Non-Functional Requirements</a> (NFRs)
* peer reviews
* pair programming
* coding standards
* architecture reviews
* code analysis tools
* automated testing
* performance and scalability testing
* dedicated testers
* defect metrics
* audits
* checklists

How many of these practices you want or need, and in what measure, are questions that will require some judgment on the part of leadership and the development team. As with many of these Big Ideas, getting the right [balance][] is not an exact science.

One thing that might help is to have at least a conceptual discussion about the <a href="http://en.wikipedia.org/wiki/Quality_costs" class="reflink" target="ref">Cost of Quality</a>. Although it is not often practical to calculate such a cost with any precision, the idea of trying to minimize the overall "COQ" is still a useful concept for consideration by teams and organizations. Introducing elements of a quality program may prove controversial, but people should be able to reach some common ground once they agree that the overall goal is to reduce the total cost of quality, including both costs of appraisal and prevention, as well as direct and indirect costs associated with software failures.

Preventive practices need not be time-consuming or costly. In many cases just asking people whether they have done something, or asking them to fill out a form attesting that they have done something, or asking for evidence that they have done something, often has an almost magical ability to influence behavior. Because, as much as we hate to admit it, if leadership does not invest the time and effort to perform such oversight, the implicit message is that they don't really want people to take the time to do these things. This impression is not the result of some vast conspiracy, or a colossal misunderstanding of management's true intentions. It is simply the case that all the very real pressures to maximize short-term benefits will inevitably influence practitioners to reduce long-term benefits, unless there is some effective counterweight.

Much of what I'm saying here is confirmed by a fascinating book by Atul Gawande called <cite>[The Checklist Manifesto: How to Get Things Right][gawande-2011]</cite>. (An <a href="http://www.npr.org/templates/story/story.php?storyId=122226184" class="reflink" target="ref">interview with Gawande</a> on the subject of his book is available from NPR.) Gawande is a surgeon, and his book is based on data from doctors and hospitals, but it turns out that surgeons are a lot like software developers: highly trained, highly experienced, and performing complex work in which no two problems turn out to be exactly alike.

When asked to consider the use of simple checklists, Gawande reports that most surgeons felt that such things were beneath them, constituted meaningless paperwork, and were a waste of time.

When they actually used them, though, amazing things happened. In one study, a hospital implemented a simple checklist to perform a series of steps to reduce the chances of patients becoming infected by insertion of central lines to supply intravenous fluids. None of the individual steps were remarkable, and all the surgeons were already familiar with all of the steps. Nonetheless, when the checklist was used consistently over a two-year period -- and when nurses were given the authority to stop doctors if they observed them to be skipping any of the steps -- the hospital calculated that, as a direct result, *use of the checklists had prevented forty-three infections and eight deaths and saved two million dollars*.

So it turns out that <a href="http://en.wikipedia.org/wiki/Watts_Humphrey" class="reflink" target="ref">Watts Humphrey</a> summarized the situation pretty well back in 1989, in <cite>[Managing the Software Process][humphrey-1989]</cite>:

> It is hard for anyone to be objective about auditors. We generally do our own jobs pretty carefully and resent any contrary implication. The need for "outside" review, however, is a matter of perspective. Suppose you had just packed a parachute and were about to take a jump. The odds are you would be happy to have a qualified inspector monitor your every step to make sure you did it just right. When quality is vital, some independent checks are necessary, not because people are untrustworthy but because they are human. The issues with software are not whether checks are needed, but who does them and how.

Gawande's book confirms Humphrey's analysis. Before running his tests, most surgeons thought the checklists were a waste of time. After having a chance to use them and see the results, 80% of the doctors thought they were something they wanted to continue to use. The other 20%, though, remained strongly against it.

But then the researchers asked one more question:

"If you were to have an operation, would you want the checklist?"

Ninety-four percent of the doctors then answered in the affirmative.

For further discussion on the topic of software quality, see the Pagan Tuna post, &ldquo;<a href="http://www.pagantuna.com/posts/software-defects.html" class="reflink" target="ref">Software Defects</a>.&rdquo;

----

<blockquote>
<p>
Let&#8217;s make toast the American way: I&#8217;ll burn, you scrape.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/W._Edwards_Deming" class="reflink" target="ref">W. Edwards Deming</a> from the article <cite>Harvard Business Review</cite>, &#8221;Quality Comes to City Hall&#8221; (March-April 1991)
</p>
</blockquote>

----

<blockquote>
<p>
Fact 37: Rigorous inspections can remove up to 90% of errors from a software product before the first test case is run.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Robert_L._Glass">Robert L. Glass</a> from the book <cite><a href="bibliography.html#glass-2003">Facts and Fallacies of Software Engineering</a></cite> Copyright &copy; 2003 by Pearson Education, Inc
</p>
</blockquote>

----

<blockquote>
<p>
You get what you design for. Chester, your peer in Development, is spending all his cycles on features, instead of stability, security, scalability, manageability, operability, continuity, and all those other beautiful &#8216;ilities.&#8217; </p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Gene_Kim">Gene Kim</a>, <a href="http://en.wikipedia.org/wiki/Kevin_Behr">Kevin Behr</a> and <a href="http://en.wikipedia.org/wiki/George_Spafford">George Spafford</a> from the book <cite><a href="bibliography.html#kim-et-al-2013">The Phoenix Project: A Novel About IT, DevOps, and Helping Your Business Win</a></cite> (2013)
</p>
</blockquote>

[balance]: software-development-is-a-balancing-act.html
[gawande-2011]: bibliography.html#gawande-2011
[humphrey-1989]: bibliography.html#humphrey-1989
[wrong]: consider-what-might-go-wrong.html

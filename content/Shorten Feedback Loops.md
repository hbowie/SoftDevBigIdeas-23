Title:  Shorten Feedback Loops

Level:  1 - Book

Timestamp: 20160503170818

Index:  Agile Manifesto; MVP (http://www.disciplinedagiledelivery.com/defining-mvp/); Minimal Viable Product (http://www.disciplinedagiledelivery.com/defining-mvp/); Mulally, Alan; Senge, Peter; demos; feedback; learning loops; retrospective (https://www.scrumalliance.org/community/articles/2014/april/key-elements-of-sprint-retrospective); 

Body:

As <a href="https://en.wikipedia.org/wiki/Alan_Mulally" class="reflink" target="ref">Alan Mulally</a> said to his team, when leading development of the Boeing 777 airliner:

> Test early and fail fast.

The feedback loops we are shortening can also be thought of as learning loops. Each loop should consist of [Plan-Do-Check-Act][pdca] steps.

Such loops can provide feedback on the product being built, or on the process being used. In Agile, process feedback is considered during a <a href="https://www.scrumalliance.org/community/articles/2014/april/key-elements-of-sprint-retrospective" class="reflink" target="ref">retrospective</a>, while product feedback is considered as part of a <a href="http://agileforall.com/how-to-give-a-great-sprint-demo/" class="reflink" target="ref">software demo</a>.

In waterfall style development, it can take the entire length of your project to obtain feedback on your product and your processes.

Agile, on the other hand, states as its third [principle][beck-et-al-2001-p]:

> Deliver working software frequently, from a couple of weeks to a couple of months, with a preference to the shorter timescale.

This practice of [delivering early and often][deliver] allows for frequent, iterative learning about customer requirements and preferences, product successes and shortcomings, as well as processes, tools and methods.

When developing a new piece of software, the best way to shorten your feedback loop is to focus your initial efforts on a <a href="http://www.disciplinedagiledelivery.com/defining-mvp/" class="reflink" target="ref">Minimal Viable Product</a> (MVP). 

<blockquote>
<p>
A Minimal Viable Product is that version of a new product which allows a team to collect the maximum amount of validated learning about customers with the least effort.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Eric_Ries">Eric Ries</a> from the book <cite><a href="bibliography.html#ries-2011">The Lean Startup: How Today's Entrepreneurs Use Continuous Innovation to Create Radically Successful Businesses</a></cite> Copyright &copy; 2011
</p>
</blockquote>

When considering feedback loops, we must be careful to make a distinction between meaningful feedback and the other kind.

Meaningful feedback on a software development project might include evaluation of results from the following activities:

* developer reports on the progress of a task, and any problems encountered;
* build of an entire system, including new code recently added;
* execution of code;
* completion of a suite of validation tests;
* demonstration of working software;
* disposition (approval or rejection) of working software by a customer;
* usage of a system by representative users attempting to perform some common tasks;
* results from completion of a coding effort, in terms of items completed; vs. items planned, and actual schedule vs. planned schedule;
* actual usage of software by real users for real tasks.

I call these items meaningful because they all should produce fairly clear and unambiguous results.

Practices such as continuous build integration, automated testing, software prototyping, daily stand-up meetings, and short rapid delivery cycles are all ways to shorten loops that produce meaningful feedback.

The other sort of feedback frequently sought on development projects comes from reviews of documents by management, management delegates, and/or professed experts. Before attempting to defend the significance of such reviews, you may wish to consider this text from <a href="http://en.wikipedia.org/wiki/Daniel_Kahneman" class="reflink" target="ref">Daniel Kahneman</a>&#8217;s 2011 book <cite><a href="bibliography.html#kahneman-2011">Thinking, Fast and Slow</a></cite>:

> In the slim volume that he later called &#8216;my disturbing little book,&#8217; [Paul] Meehl reviewed the results of 20 studies that had analyzed whether clinical predictions based on the subjective impressions of trained professionals were more accurate than statistical predictions made by combining a few scores or ratings according to a rule. In a typical study, trained counselors predicted the grades of freshmen at the end of the school year. The counselors interviewed each student for forty-five minutes. They also had access to high school grades, several aptitude tests, and a four-page personal statement. The statistical algorithm used only a fraction of this information; high school grades and one aptitude test. Nevertheless, the formula was more accurate than 11 of the 14 counselors. Meehl reported generally similar results across a variety of other forecast outcomes, including violations of parole, success in pilot training, and criminal recidivism.

Kahneman goes on to point out that:

> Another reason for the inferiority of expert judgment is that humans are incorrigibly inconsistent in making summary judgments of complex information. When asked to evaluate the same information twice, they frequently give different answers.

So take results from these sorts of reviews with a grain of salt. You may get some enlightening feedback that will prove helpful, but you are just as likely to get confusing direction that can lead you down the garden path. 

----

<blockquote>
<p>
The most powerful learning comes from direct experience. But what happens when we can no longer observe the consequences of our actions? Herein lies the core <em>learning dilemma</em> that confronts organizations:<em> we learn best from experience but we never directly experience the consequences of many of our most important decisions.</em> </p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Peter_Senge" class="reflink" target="ref">Peter Senge</a> from the book <cite><a href="bibliography.html#senge-1990">The Fifth Discipline: The Art and Practice of the Learning Organization</a></cite> Copyright &copy; 1990 by Peter M. Senge.
</p>
</blockquote>



[beck-et-al-2001-p]: bibliography.html#beck-et-al-2001-p
[deliver]: deliver-early-and-often.html
[pdca]: plan-do-check-act.html

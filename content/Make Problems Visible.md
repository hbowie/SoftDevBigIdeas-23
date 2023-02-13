Title: Make Problems Visible

Index: problems
Index: problem-solving
Index: code reviews
Index: automated testing
Index: user demos
Index: lean
Index: visibility
Index: Toyota
Index: Fackler, Martin

Body:

Any software development project can be thought of as a series of problems to be solved. [Planning][plan] can help a [team][teams] anticipate problems, but the discovery and solving of problems is a process that continues over the life of the project.

When a new problem is discovered, it's best to avoid the following sorts of dysfunctional behavior:

* Shoot the messenger who reported it;
* Ignore the problem in hopes it will go away;
* Stick your head in the sand and wait for someone else to notice the problem;
* Find someone to blame for causing the problem.

As new problems are discovered, instead of falling back on any of these behaviors, it is important to accept the problems as part of the work that needs to be done.

The longer software problems fester, the more expensive they will be to solve, so it is best to face into them and address them early.

This is one reason why code reviews, automated testing, user demos and frequent releases are all good ideas: all of these practices tend to make problems visible before they become more serious, and more difficult to rectify.

Another benefit of early discovery of problems is that it is generally easier for team members at this point to understand how and why they occurred, and to figure out how to reduce the likelihood of similar problems in the future.

Note that making problems visible is a central tenet of <a href="https://en.wikipedia.org/wiki/Lean_manufacturing" class="reflink" target="ref">Lean</a>, as indicated in this New York Times article from 2007:

<blockquote>
<p>
&#8220;For Americans and anyone, it can be a shock to the system to be actually expected to make problems visible,&#8221; said Ms. Newton, a 38-year-old Indiana native who joined Toyota after college 15 years ago and now works at the North American headquarters in Erlanger, Ky. &#8220;Other corporate environments tend to hide problems from bosses.&#8221; </p>

<p>
&#8220;Mutual ownership of problems,&#8221; is one slogan. Other tenets include &#8220;genchi genbutsu,&#8221; or solving problems at the source instead of behind desks, and the &#8220;kaizen mind,&#8221; an unending sense of crisis behind the company&#8217;s constant drive to improve. </p>

<p>
…some executives like Mr. Konishi complain of managers at Toyota factories who have not adhered to some of the company&#8217;s most basic creeds, like allowing workers to stop factory lines when they spot defects. Empowering factory workers has long been central to Toyota&#8217;s quality control.</p>

<p class="bq-footer">
Martin Fackler from <cite><a href="bibliography.html#nytimes-2007">The New York Times</a></cite>, &#8221;The ‘Toyota Way’ Is Translated for a New Generation of Foreign Managers&#8221; (Feb 15, 2007)
</p>
</blockquote>

As indicated in this quotation, people will not make problems visible if this results in them being punished for making mistakes. In order to surface problems, the organizational culture must support mutual ownership of problems, and focus on fixing the problems rather than assigning blame.

In some ways, this can be thought of as a reversal of the perspective adopted by most organizations.

![Lean Model Diagram](images/a-new-model-for-lean-culture.jpg "Traditional vs. Lean Cultures")

In traditional thinking, the emphasis is first and foremost on putting various organizational structures in place -- tools, systems, org charts, budgets, plans, performance objectives, etc. -- then on coaching people for conformance to those structures, with problems viewed primarily as issues of non-conformance to the structures: mistakes that would not have happened if people had just been following the instructions they had been given.

In lean thinking, this emphasis is reversed. Solving problems is viewed as a primary function for all workers, people are coached to enhance their problem-solving skills, and fluid structures are created and modified to adapt to emergent problems and their solutions.

For more on this topic, see the Pagan Tuna post, &ldquo;<a href="http://www.pagantuna.com/posts/a-new-model-for-lean-culture.html" class="reflink" target="ref">A New Model for Lean Culture</a>.&rdquo;

[lc]: http://www.pagantuna.com/posts/a-new-model-for-lean-culture.html

[nytimes-2007]: bibliography.html#nytimes-2007
[plan]: plan-thoughtfully-but-be-prepared-for-change.html
[teams]: build-great-teams.html

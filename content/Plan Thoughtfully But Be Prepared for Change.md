Title: Plan Thoughtfully But Be Prepared for Change

Index: Agile Manifesto
Index: Berkun, Scott
Index: Eisenhower, Dwight D.
Index: Kennedy, Michael N.
Index: MVP (http://www.disciplinedagiledelivery.com/defining-mvp/)
Index: Miller, Henry
Index: Minimal Viable Product (http://www.disciplinedagiledelivery.com/defining-mvp/)
Index: Robertson, James and Suzanne
Index: capacity allocation (http://www.scaledagileframework.com/team-backlog/)
Index: change
Index: elephant
Index: horse
Index: innovation
Index: planning
Index: rabbit
Index: roadmap (http://www.scaledagileframework.com/roadmap/)

Body:

<blockquote>
<p>
In preparing for battle, I have always found that plans are useless but planning is indispensable.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Dwight_D._Eisenhower" class="reflink" target="ref">Dwight D. Eisenhower</a> from the book <cite><a href="bibliography.html#nixon-1962">Six Crises</a></cite> (1962)
</p>
</blockquote>

Planning is an essential activity for any project, because it helps developers anticipate problems and prepare ways to address them.

Are there key constraints that must be applied to your project, related to budget, resources, or schedule? Are there specific design constraints that must be respected? Make sure you understand these thoroughly and plan accordingly.

It's good to establish an implementation strategy and roadmap for your project at this point. What is the <a href="http://www.disciplinedagiledelivery.com/defining-mvp/" class="reflink" target="ref">Minimal Marketable Product</a> (MMP) that can usefully be released to your customers? How can additional functionality be added in an incremental fashion? What are the dependencies between various features, or groups of features? These are the sorts of considerations that will help you define your implementation strategy.

Your <a href="http://www.scaledagileframework.com/roadmap/" class="reflink" target="ref">roadmap</a> should show your planned releases, along with other key project milestones, laid out across an approximate timeline. The number of releases and the timeframe depicted should reflect known stakeholder agreements and negotiated expectations. The timeframe should not be arbitrarily shortened, if doing so would allow the team to lose sight of critical milestones farther in the future.

It's also good at this point to consider any key requirements challenges. Are there certain areas of the project where requirements are likely to be hard to define? Perhaps areas where different stakeholders have conflicting requirements? Or areas where important stakeholders will be difficult to meet with regularly? If you can anticipate areas where requirements definition will be challenging, then you should plan time and resources to work these issues before trying to work them out during a coding iteration.

You should also try to anticipate any significant [design][] challenges. Are there any areas of your system that will need concentrated design attention? These may be areas of UI design, or areas of database design, or areas of application architecture, or application integration, or some combination of these and perhaps other areas. They may need special attention because certain requirements do not have straightforward solutions, or because certain design elements represent opportunities for achieving fresh and innovative solutions that will deliver significant additional value to your customers. In any of these cases, you should plan additional time and resources to work these design problems before throwing related user stories into a development iteration.

Make sure you plan sufficient time and resources to produce all relevant and required documentation. James and Suzanne Robertson have pointed out that a project can be classified as [a rabbit, a horse, or an elephant][robertson-1999], depending on the degree of formality needed for its requirements documentation. This need is often dictated by factors outside of the control of the project team. Similarly, in any large enterprise, there will likely be some significant expectations for architecture documentation, and again, these documentation requirements will not easily be wished away.

You should also think about your presumed technology stack and its readiness. Be explicit and transparent about the technologies you intend to use, including application components and development tools. Be wary of any technical paths that may be candidates for severe disruption over the course of your project or over the intended life of your product. Lay out enough of your intended application architecture to show how these technologies will be used within the context of your solution. Ensure all key stakeholders, including those in architecture oversight roles, endorse your decisions, and make sure someone records these decisions and approvals in some sort of permanent record.

Then assess the readiness of the technology for use by your development team. Is the stack already proven? Is the team already familiar with it? If you answer either of these questions in the negative, then be sure to factor additional time into your plan to allow for technical experimentation and/or training.

This is also a good time to establish initial agreements on <a href="http://www.scaledagileframework.com/team-backlog/" class="reflink" target="ref">capacity allocation</a> for your team members. Your development team will spend most of its time developing new features. But over the long haul it will realistically also need to spend some of its time on defect correction, as well as refactoring, design improvements, and technology upgrades. The best way to address the need to include these unlike things in your development work is by use of capacity allocation. You can renegotiate the percentages allocated to different types of work over time, but it's best to introduce the concept early, establish some starting agreements, and then bake these into your planning assumptions so that you don't over-estimate your development capacity.

You should also plan for time to be spent on integration and hardening. Will you have one or more teams working semi-independently on different pieces of your system? If so, be sure to factor in time and resources for integration testing and hardening of the integrated solution. This may come in the form of a periodic hardening sprint, or additional integration work as part of each development sprint. However you incorporate it into your plan, though, such work will consume additional time that would otherwise be available for development of new features.

All of these factors, as well as others, should be considered as part of your initial planning.

However, plans should never be regarded as written in stone. They are always works in progress, and always subject to further change.

The [Agile Manifesto][beck-et-al-2001] expresses this idea by stating that its signatories value "responding to change over following a plan."

<a href="http://en.wikipedia.org/wiki/Michael_N._Kennedy">Michael N. Kennedy</a> says something similar in his book, <cite><a href="bibliography.html#kennedy-2003">Product Development for the Lean Enterprise</a></cite>:

> Product development by its nature is a &#8220;reactive&#8221; process, and cannot be managed as if it is &#8220;transactional&#8221;.

----

<blockquote>
<p>
The dirty little secret &#8212; the fact often denied &#8212; is that unlike the mythical epiphany, real creation is sloppy. Discovery is messy. Exploration is dangerous.</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Scott_Berkun">Scott Berkun</a> from the book <cite><a href="bibliography.html#berkun-2007">The Myths of Innovation</a></cite> (2007)
</p>
</blockquote>

----

<blockquote>
<p>
Plot, plan, calculate or postulate as we may, there will always be surprises in store for us. Count on it!</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Henry_Miller">Henry Miller</a> from the book <cite><a href="bibliography.html#miller-1962">Stand Still Like the Hummingbird</a></cite> Copyright &copy; 1962 by Henry Miller
</p>
</blockquote>



[beck-et-al-2001]: bibliography.html#beck-et-al-2001

[0]: http://en.wikipedia.org/wiki/Dwight_D._Eisenhower
[nixon-1962]: bibliography.html#nixon-1962
[2]: http://en.wikipedia.org/wiki/Henry_Miller
[miller-1962]: bibliography.html#miller-1962
[kennedy-2003]: bibliography.html#kennedy-2003
[mnk]: http://www.targetedconvergence.com/about-tcc/our-people/michael-n-kennedy-founder-.html

[capalloc]: http://www.scaledagileframework.com/team-backlog/
[design]:   just-enough-design-up-front.html

[robertson-1999]: bibliography.html#robertson-1999

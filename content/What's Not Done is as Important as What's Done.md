Title: What's Not Done is as Important as What's Done

Index: not done; undone
Index: YAGNI
Index: prioritization
Index: governance

Body:

Quite naturally, we often look at software development as the process of doing stuff, of creating new things, of generating new features for our customers.

And our enthusiasm for doing things, for making customers happy, can lead us to create lots and lots of new things.

Let's think for a minute, though, about the costs of creating each new thing:

1. Doing the initial coding;
2. Further refining the code in response to customer feedback;
3. Testing and debugging the code;
3. Reviewing the new code and performing quality checks on it;
4. Integrating the code into the larger environment;
5. Applying coding standards and Non-Functional Requirements to the new code;
6. Documenting the new thing, both for users and for system maintainers;
7. Training users on the new thing;
8. Future regression testing, to make sure the new thing continues to work as other software continues to evolve;
9. Increased system maintenance costs, due to overall increased complexity of the software;
10. Future maintenance of the new thing, as customer needs and desires continue to evolve;
11. Work to replace the new thing, when it comes time to replace the current system with something newer and more modern.

Of course, when we're considering development of that new thing -- whether it's a new application or a new feature -- we often think only of the cost of item 1, the initial coding, even though we can clearly see that this is only the tip of a very large iceberg.

So what is the alternative? What can we do instead of developing that new thing, in order to save all this cost?

* If the need for the new thing is not immediate, then assume for the time being that <a href="https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it" class="reflink" target="ref">You Ain't Gonna Need It</a> (a principle often abbreviated as "YAGNI").
* Suggest the customer use another application or feature [that already exists][reuse].
* [Simplify and generalize][simplify] existing code to accommodate the intent of the new feature.
* Do something else that is more important.

In order to exercise this last option, of course, you will need some means of establishing the priority of this thing compared to other things of a similar nature. And here we run into another strong reason for [Delivering Early and Often][deliver]. If your project will only have one large monolithic delivery, then it will be pretty hard to get anyone to admit that any of the proposed features don't deserve to be included, and so you will end up with everything on your list, up to and including the proverbial kitchen sink.

On the other hand, if you are delivering new software every 1 - 4 weeks, in a regular, repeatable cadence, then it will be much easier to get agreement on what is to be included in the next sprint, since other items are not being dropped forever, but only left on the backlog for consideration again in a few more weeks.

At some point, of course, you will have implemented the most valuable features, and will only have low-value features left in the backlog. At this point, your [governance][govern] process should kick in, and divert your available investment dollars to some other project, so that your organization can continue to maximize the [value being created for your customers][value].


[deliver]: deliver-early-and-often.html
[govern]: govern-wisely.html
[reuse]: use-things-already-known-to-work.html
[simplify]: simplify-and-generalize.html
[value]: create-value-for-customers.html


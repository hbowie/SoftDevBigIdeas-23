Title: Configuration Management

Index: configuration management (https://en.wikipedia.org/wiki/Configuration_management)
Index: change management
Index: version control
Index: CM (https://en.wikipedia.org/wiki/Configuration_management)
Index: separation of duties (https://en.wikipedia.org/wiki/Separation_of_duties)
Index: SoD (https://en.wikipedia.org/wiki/Separation_of_duties)
Index: DevOps
Index: Kim, Gene
Index: Behr, Kevin
Index: Spafford, George

Body:

As with many safety and quality practices, <a href="https://en.wikipedia.org/wiki/Configuration_management" class="reflink" target="ref">configuration management</a> is often most visible by its absence.

As in...

> What do you mean, you can't find the source code?

Or...

> You know that nasty bug we discovered last week?
>
> Well, that's been fixed now.
>
> Unfortunately, we've also somehow lost the last three enhancements we made.

While the following list of suggested CM practices is not exhaustive, it's a good place to start.

1. Make sure you have multiple backups of your source code -- in development as well as in production.

2.  Use a version control system that automatically maintains prior versions of all of your programs and modules.

3.  For each release of your application, maintain a complete list of all the application's components, with the version level of each.

4. Always create executables to be released via an automated build process using configuration-controlled source code.

5. Maintain records that always allow you to trace back from any given change in the source code to the original request that provided the rationale for the change.

6. Always maintain some <a href="https://en.wikipedia.org/wiki/Separation_of_duties" class="reflink" target="ref">separation of duties</a> (SoD) between the developers and the folks responsible for implementing a release to production.


----

<blockquote>
<p>
Chris seems excited. &#8220;Brent, if it&#8217;s okay with you and everyone else, I&#8217;d like to invite you to our team sprints, so that we can get environment creation integrated into the development process as early as possible. Right now, we focus mostly on having deployable code at the end of the project. I propose we change that requirement. At each three-week sprint interval, we not only need to have deployable code but also the exact environment that the code deploys into, and have that checked into version control, too.&#8221;</p>

<p class="bq-footer">
<a href="http://en.wikipedia.org/wiki/Gene_Kim">Gene Kim</a>, <a href="http://en.wikipedia.org/wiki/Kevin_Behr">Kevin Behr</a> and <a href="http://en.wikipedia.org/wiki/George_Spafford">George Spafford</a> from the book <cite><a href="bibliography.html#kim-et-al-2013">The Phoenix Project: A Novel About IT, DevOps, and Helping Your Business Win</a></cite> (2013)
</p>
</blockquote>


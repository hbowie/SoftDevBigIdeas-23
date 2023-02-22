Title:  Configuration Management

Seq:    6.4

Idea Number: 42

Level:  3 - Article

Class:  article

Timestamp: 20160601214652

Index:  configuration management (https://en.wikipedia.org/wiki/Configuration_management); change management; version control; CM (https://en.wikipedia.org/wiki/Configuration_management); separation of duties (https://en.wikipedia.org/wiki/Separation_of_duties); SoD (https://en.wikipedia.org/wiki/Separation_of_duties); DevOps; Kim, Gene; Behr, Kevin; Spafford, George; 

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

##### Words from Others on this Topic

{:include-quote:Integrate environment creation into the development process}


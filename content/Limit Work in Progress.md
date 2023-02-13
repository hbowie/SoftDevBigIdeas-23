Title: Limit Work in Progress

Index: WIP
Index: work in progress
Index: task switching (https://en.wikipedia.org/wiki/Task_switching_(psychology))
Index: surge capacity
Index: capacity allocation

Body:

In many software development environments, new requests seem to continually arrive in an uncontrolled fashion. The result can often be that work on the latest request interrupts completion of work that arrived earlier, so that all requests tend to take longer to complete, and the total amount of work-in-progress (WIP) increases, making it exponentially more difficult to manage.

Such an uncontrolled intake process also tends to reduce overall developer productivity, since developers spend more time <a href="https://en.wikipedia.org/wiki/Task_switching_(psychology)" class="reflink" target="ref">task switching</a>, and less time actually doing productive development.

This is why it is generally critical to limit the entry of new requests into an active in-work state. There are various approaches to implementing such limits, but one of them should generally be adopted in any active development environment.

One approach is to set specific numeric limits on the number of items that can be in work at any point in time, so that new items are started only as other items are completed.

When implementing such a system, it's useful to plan for some sort of surge capacity, to handle emergent high-severity bugs, and it's also useful to allocate certain percentages of your capacity to types of work other than new features for your customers -- things like refactoring, defect correction, and reduction of technical debt -- since otherwise items like these may have trouble competing successfully with new feature requests.

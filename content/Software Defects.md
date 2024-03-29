Title:  Software Defects

Tags:   Quality, Software Development

Seq:    8.11

Level:  3 - Article

Class:  article

Timestamp: 20230217233540

Body:

Some of the most troublesome topics in software development are those surrounding defects:

* Why do defects happen?
* How can we prevent them?
* Can they be eliminated?
* What metrics can we use to measure our success (or lack thereof)? 

Let me introduce my thoughts on this topic with a little story.

When I started my career, programmers were still using coding sheets that were sent to keypunch operators to be converted into punched cards. The card decks were then sent to a mainframe to be compiled. There were few if any defects introduced by the keypunch operators, because at that time every punched card was independently verified by another operator, who essentially re-keyed every character on every line of every coding sheet. So the first set of errors, or defects, that a programmer normally had to deal with were the syntax and spelling errors found by the compiler. 

My programming group at that time had one member who was known for first-time quality. He performed extensive desk checks of his coding sheets before sending them to keypunch, and as a result almost all of his programs sailed through the compilation step without generating any errors at all. 

Of course, if you ever went out to lunch with this guy, you would discover that he never made a left-hand turn, but instead would invariably make three right-hand turns, because that way he never had to turn in front of oncoming traffic! 

If I seem to be boring you with ancient personal history, it's only because the simple story above illustrates most of the basic issues still surrounding software defects today. 

1. Humans will make errors. 

2. There are various types of errors that can be made. 

3. Many forms of defect prevention require an explicit inspection of the original work, either by the original worker or by a peer. 

4. Automation should be used as much as possible to prevent as many types of errors as practical. 

5. The sooner an error can be detected and corrected, the cheaper it will be to fix. 

6. There are trade-offs to be made between the costs of prevention and the risks of failures; risks should be reduced to a reasonable level, but the costs of prevention should not become unreasonable in the process. 

All of this sounds pretty straightforward, and yet issues surrounding defects still seem to regularly generate lots of controversy in software development discussions. 

Here are a few general recommendations.

## 1. Use the Cost of Quality as a conceptual model.

Although it is not often practical to calculate such a cost with any precision, the idea of trying to minimize the overall "[Cost of Quality](http://en.wikipedia.org/wiki/Quality_costs)" is still a useful concept for consideration by teams and organizations. Discussing test automation, peer reviews, and pair programming may prove controversial, but people should be able to reach some common ground once they agree that the overall goal is to reduce the total cost of quality, including both costs of appraisal and prevention, as well as direct and indirect costs associated with software failures. 

## 2. Allow the development team to self-manage defects that are contained within the team.

It is occasionally tempting for upper management or well-intended governance bodies to try to mandate certain internal quality (i.e., defect prevention) practices and metrics across an entire software organization. This may work well if all the teams are really doing very similar kinds of work on pieces of a unified product, but in other situations (such as many large and diverse IT organizations), my strong sense is that such policies do more damage, in terms of compromising each team's sense of autonomy, than they do good. It is easier to measure a team's performance in terms of productivity or cycle time than to try to make some meaningful sense of how each team internally deals with defect identification and correction. 

## 3. Do not confuse consideration of design alternatives with rework. 

Many projects can benefit from some quick elaboration of design alternatives (aka rapid prototyping) in order to allow stakeholders to more meaningfully evaluate those alternatives. Even though this may result in some work being "thrown away," none of this should be treated as work associated with the creation or correction of defects. Such work is part of the cost of design, not the cost of quality. 

Unfortunately, many agile teams simply treat consideration of design alternatives as something that is part and parcel of their iterative development process; this is unfortunate because it then becomes difficult to disentangle team design and quality practices in any meaningful manner. If you're in a situation where all software changes (including correction of defects and changes in design) are simply treated as more grist for the development team's backlog, then you know you're in this situation, and you should try to get out of it. 

## 4. Focus organizational attention on defects that impact others outside of the dev team.

Defects that "escape" from a dev team and cause negative impacts to others (customers, users, integrated test teams, etc.) should be rigorously measured and tracked and managed at an organizational level. 

## 5. Differentiate between varying severity levels. 

All defects are not created equal. Any sort of reporting and metrics systems should be sure to assign appropriate weights to defects based on their severity. While wording may vary, a scale similar to the following is often used. 

1. The system was rendered totally inoperable or unusable. 
2. A significant portion of the system was unavailable or unusable. 
3. The entire system was available and usable, but with some significant degradation of performance or functionality. 
4. Problems were only cosmetic in nature. 

## 6. Perform causal analysis for quality escapes. 

For software defects that escape into the wild, it is useful to ask why they happened, and what could have prevented them. 

This sort of analysis is typically referred to as [Root Cause Analysis](http://en.wikipedia.org/wiki/Root_cause_analysis), however the focus should not be on coming up with a single root cause, but with as many actionable causes as possible, along with reasonable actions that will reduce the likelihood of recurrence of the same or similar problems in the future. 

When performing this sort of causal analysis, it may be useful to ask a more specialized variation of the usual [Five Whys](http://en.wikipedia.org/wiki/5_Whys) that are typically invoked for this sort of work. 

* Why did the overall system/service fail? Which component(s) (hardware, network, system software, application software, etc.) were at fault?

* Why is this problem considered a defect? Was it a sin of omission, an error in the way a feature was implemented, or an additional feature that was not requested? 

* What sorts of problems were noted? Did the system crash, or fail to operate at all? Or did it run, but with degraded performance? Or were the problems functional, rather than operational?

* Why did the failure occur at this point in time? Was it caused by a recent change to the software? Or a recent change to the infrastructure? Or a change in user processes and practices? 

* Were there integration issues between components? In other words, did the components appear to operate correctly when tested independently, but fail when used in combination? If so, why weren't these integration issues identified and addressed earlier?

* Were there unanticipated changes in functional or operational expectations for the software? In other words, did the requirements change without those responsible for the software knowing about the change? If so, then why weren't the changing requirements communicated?

* Why weren't the defects discovered during testing?  

* If the defect occurred because of recent changes to the software, then why was the defect introduced? Was it injected during coding (a coding error), during design (a design error), or during requirements elicitation and definition (a requirements error)? What would help prevent recurrence in the future? Is further education needed? Or additional reviews of code and/or documents? Are there automated tools that can help? 

If you ask these questions, and get some reasonable answers, then you should be able to identify some meaningful actions to be taken to help prevent a recurrence of similar sorts of problems in the future. 

## 7. Make metrics simple and meaningful. 

It would certainly be possible to create a comprehensive system of data collection and metrics reporting that would answer all possible questions about all defects found and corrected for any particular set of systems. But the necessary level of effort might not actually provide any commensurate level of benefits. 

Again, my advice would be to make a clean separation between defects caught internally, vs. quality escapes. For the former, I would suggest that each development team be allowed to establish and track their own metrics. 

For quality escapes, my advice would be to use something like the [GQM](http://en.wikipedia.org/wiki/GQM) (Goal-Question-Metric) approach in order to provide focus for your metrics collection and reporting efforts. In other words, start with a goal, or a small number of goals. For each goal, what sort of questions would you like to be able to answer to find out how you're doing on the way to meeting that goal? And then what metrics will help you answer those questions? 

----

The first programmers were able to blame their problems on actual insects crawling around inside their computing hardware; these days, however, everyone knows that software bugs should not be treated as a branch of entomology. How they should be treated, however, is often a topic of much debate. Hopefully the comments above can help to steer such conversations into productive channels.

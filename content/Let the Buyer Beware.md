Title: Let the Buyer Beware

Index: COTS
Index: suppliers
Index: vendors
Index: caveat emptor
Index: customization
Index: purchased software
Index: ISV
Index: independent software vendor
Index: Hurst, Mark

Body:

While there are certainly advantages to buying software rather than building it, buyers must be careful that the software they are acquiring is a good fit for their needs, and that that the long-term interests of the software supplier (whether commercial or open source) overlap sufficiently with the buyer's interests.

Too often we in IT seem to be lured by the promise of off-the-shelf functionality whose development costs will be spread over a large customer base, yet end up with purchased software that we then have to modify or extend to fit our special requirements, ensuring that we end up with the worst of both worlds.

Here are some key issues to be considered before purchasing a Commercial Off the Shelf (COTS) software package.

**1. Can system requirements be based on some set of rules that are generally accepted by industry?**

As an example, a computer-aided design (CAD) system is based on certain rules of geometry -- pretty hard for a user to insist that these need to be customized! Similarly, an application like <a href="http://www.turbotax.com" class="reflink" target="ref">TurboTax</a> is based on a particular country's tax code -- which would make it hard to justify the internal development of a custom system to perform a similar function. Another example would be a <a href="http://en.wikipedia.org/wiki/Material_requirements_planning" class="reflink" target="ref">Materials Requirements Planning</a> (MRP) system, which can rely on standard practices defined by the <a href="http://www.apics.org" class="reflink" target="ref">APICS</a> organization.

In my experience, COTS packages that are largely based on standard sets of rules such as these are frequently well accepted by users and developers, while others with more variable or controversial requirements are not.

**2. How hard would it be to develop the system internally?**

If the system that is needed is relatively simple, without any significant technical challenges, then a COTS solution is often expensive overkill, especially if you will be paying for more bells and whistles and configuration options than you really have any use for.

Notice that the answer to this question may well change over time, as new technical capabilities become more generally available through various layers of infrastructure software.

**3. Can the business benefit from a rapid response to requests for functional enhancements?**

Cycle times for changes to COTS software -- measured from concept to cash, from original idea to working software in the hands of users -- can often be an order of magnitude longer than for internally developed systems.

**4. Will the internal integration requirements be so complex that upgrades to future releases of the application will be virtually impossible?**

Customers often optimistically expect to be able to benefit from future releases of an application, but in practice, the web of connections to other applications becomes so complex over time that the costs of implementing a new release often outweigh the benefits. And even when these connections start out being well managed by IT, interfaces with user-developed software and data stores often overwhelm the best laid IT architecture.

**5. Is there a viable business model for an <a href="http://en.wikipedia.org/wiki/Independent_software_vendor" class="reflink" target="ref">independent software vendor</a> (ISV) to produce the desired system over the long haul?**

Companies routinely assess the financial stability of potential suppliers, but often fail to question the long-term viability of a vendor's business model. What matters is not how many customers and how much cash in the bank they have today, but how they will maintain those numbers over time. As a notorious example, suppliers that market software specifically designed for government contractors tend to go belly-up with disturbing regularity.

**6. Will a unique, internally developed system provide us with some lasting advantage over our competitors?**

The alternative would be that we only need a system that is as good as similar systems used by our competitors. If our goal is only parity, then an internally developed system might actually be wasteful, since we may spend time dreaming up unique requirements that add cost but no useful business differentiation.

Consideration of these factors can often help guide a team to a make-or-buy decision that will serve its customers well over the long haul.

----

<blockquote>
<p>
It&#8217;s far too rarely stated that the technology industry is not in the business of making people productive. It is only in the business of selling more technology. Granted, some companies make better tools than others, and users can be productive with some of today&#8217;s tools. But in the technology business, users&#8217; productivity is secondary to profitability. No matter what a company claims, feature lists and upgrades are designed for the company&#8217;s success, not the users&#8217;.</p>

<p class="bq-footer">
<a href="http://creativegood.com/mark-hurst/" class="reflink" target="ref">Mark Hurst</a> from the book <cite><a href="bibliography.html#hurst-2007">Bit Literacy: Productivity in the Age of Information and E-mail Overload</a></cite> Copyright &copy; 2007 by Good Experience, Inc.
</p>
</blockquote>


# tax-min-method

What the project does and why is it useful?

https://www.betterment.com/resources/lowering-your-tax-bill-by-improving-our-cost-basis-accounting-methods/

When Betterment customers sell securities, our algorithms select which specific lots to sell on the fly, following a set of rules which we call TaxMin. This method is more granular in its approach, and will improve the tax impact for most transactions, as compared to FIFO.

How does this method work? Instead of looking solely at the purchase date of each lot, TaxMin also considers the cost basis of the lot, realizing all losses before any gains, regardless of when the shares were bought. Lots are sold in the following order:

Short-term losses Long-term losses Long-term gains Short-term gains The algorithm exhausts each category before moving to the next, but within each category, lots with the highest cost basis are sold first. With a gain, the higher the basis, the smaller the gain, which results in a lower tax burden. In the case of a loss, the opposite is true: the higher the basis, the bigger the loss (which is beneficial, since it can offset gains).

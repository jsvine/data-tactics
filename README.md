# Data Tactics

*Note: This is a half-baked draft.*

Chess players differentiate between [__tactics__](http://en.wikipedia.org/wiki/Chess_tactic) and [__strategy__](http://en.wikipedia.org/wiki/Chess_strategy). Tactics are [short sequences of moves](http://www.chessfornovices.com/chessstrategyvstactics.html): the "pin," the "skewer," and so on. They're relatively simple; you could learn them in an afternoon. Strategy, on the other hand, relates to long-term plans and takes years or decades to master. Strategy builds upon tactics, but not mechanistically. Great players distinguish themselves by cleverly combining the core tactics and thinking (far) ahead. 

Although data analysis doesn't strongly resemble chess, the strategy/tactics distinction might still be helpful. While the long-term strategies of data analysis take years to master, they're built upon simpler core tactics. This repository aims to catalog the most useful "data tactics."

The data tactics below are roughly ordered from the simplest to the most complex.

## Summarizing Tactics

Summarize a list of numbers into a single metric.

- __Count__
	- E.g., given a list of incomes for a town: *How many incomes were counted?*
- __Minimum__
	- *What's the lowest income?*
- __Maximum__
	- *What's the highest income?*
- __Sum__
	- *What's the total income among this group?*
- __Mean__
	- *What's the average income?*
- __Median__
	- *What income separates the top half of residents from the bottom half?*
- __Mode__
	- *What's the most common income?*
- [__Standard deviation__](http://en.wikipedia.org/wiki/Standard_deviation)
	- *How much does income vary from resident to resident?*

## Pairwise Tactics

Combine a pair of numbers into a single number. You can also apply pairwise tactics to two lists of numbers.

- __Subtract__
- __Multiply__
- __Divide__

## Transformational Tactics

Transform an individual bit of data into another bit of data, based on some rule.

- __Classify__ (into categories)
- __Normalize__ (text into canonical representations, e.g., "ACME, Incorporated" & "Acme, inc." -> "ACME, Inc.")
- __Resample__ (time series data, e.g., day -> month)
- __Geocode__ (addresses -> lat/long)
- __Rescale__ (e.g., into logarithmic scale)

## Comparative Tactics

Compare a number to its peers.

- __Rank__
- __Quantiles__ (e.g., percentiles)
- __Percent difference__
- __Z-score__

## Structural Tactics

Reshape or reorganize tables of data.

- __Sort__
- __Filter/subset__
- __Transpose__
- __Join__
 
## Grouping

Grouping is a tactic of its own, and the connective tissue of many analyses. In grouped, or "aggregate," analyses, you split up your data into two or more groups, and then run calculations on those subsets.

# Examples

For the following examples, we'll use the [most recent data from SupremeCourtDatabase.org](http://supremecourtdatabase.org/data.php).

- During the 2013 term, *how many* cases did the Supreme Court decide?
	- __Filter__ the data to `term`:`2013`.
	- __Count__ the number of cases that remain.

- During the 2013 term, *how many* cases did the Supreme Court decide 9-0?
	- __Filter__ the data to `term`:`2013`.
	- __Filter__ again, to `majVotes`:`9`.
	- __Count__ the number of cases that remain.

- During which term, 1946–2013, did the Supreme Court decide the most 9-0 cases?
	- __Filter__ the data to `majVotes`:`9`.
	- __Group__ the remaining data by `term`. With each group:
		- __Count__ the number of cases.
	- __Sort__ those counts from greatest to least.

- During which term, 1946–2013, did the Supreme Court decide the *greatest percentage* of cases by 9-0?
	- __Classify__ `majVotes` as a new column, called `nine_to_zero`, where the values are `1` (if `majVotes`:`9`) or `0` if not.
	- __Group__ all the cases by `term`. With each group:
		- Get the __mean__ of `nine_to_zero`.
	- __Sort__ those counts from greatest to least.

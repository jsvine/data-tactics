# Data Tactics

*Note: This is a half-baked draft.*

Chess players differentiate between [__tactics__](http://en.wikipedia.org/wiki/Chess_tactic) and [__strategy__](http://en.wikipedia.org/wiki/Chess_strategy). Tactics are [short sequences of moves](http://www.chessfornovices.com/chessstrategyvstactics.html): the "pin," the "skewer," and so on. They're relatively simple; you could learn them in an afternoon. Strategy, on the other hand, relates to long-term plans and takes years or decades to master. Strategy builds upon tactics, but not mechanistically. Great players distinguish themselves by cleverly combining the core tactics and thinking (far) ahead. 

Although data analysis doesn't strongly resemble chess, the strategy/tactics distinction might still be helpful. While the long-term strategies of data analysis take years to master, they're built upon simpler core tactics. This repository aims to catalog the most useful "data tactics."

The data tactics below are roughly ordered from the simplest to the most complex.

## Summarizing Tactics

Tactics that represent, in a single number, *something* about list of numbers.

- __Count__
	- E.g., given a list of incomes for a town: *How many incomes were counted?*
- __Sum__
	- *What's the total income among this group?*
- __Mean__
	- *What's the average income?*
- __Minimum__
	- *What's the lowest income?*
- __Maximum__
	- *What's the highest income?*
- __Median__
	- *What income separates the top half of residents from the bottom half?*
- __Mode__
	- *What's the most common income?*
- [__Standard deviation__](http://en.wikipedia.org/wiki/Standard_deviation)
	- *How much does income vary from resident to resident?*

## Pairwise Tactics

Tactics that work on a pair of numbers (or two lists of numbers).

- __Subtract__
- __Multiply__
- __Divide__

## Transformational Tactics

Tactics to transform individual bits of data.

- __Rescale__ (e.g., logarithm, square root, etc.)
- __Classify__
- __Reduce dimensions__
- __Extract features__
- __Normalize__ (text)
- __Geocode__ (addresses -> lat/long)
- __Resample__ (time series data, e.g., day -> month)
- __Rolling average__

## Comparative Tactics

Tactics to compare one value to a broader set of numbers.

- __Rank__
- __Quantiles__ (e.g., percentiles)
- __Percent difference__
- __Z-score__

## Structural Tactics

Tactics to reshape/reorganize data tables.

- __Sort__
- __Filter/subset__
- __Transpose__
- __Join__
 
## Combinatory Tactics

Tactics that combine two or more basic tactics.

- __Grouped summary statistics__
- __Crosstabs / pivot tables__

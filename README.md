# Data Tactics

*Note: This is a half-baked draft.*

Chess players differentiate between [__tactics__](http://en.wikipedia.org/wiki/Chess_tactic) and [__strategy__](http://en.wikipedia.org/wiki/Chess_strategy). Tactics are [short sequences of moves](http://www.chessfornovices.com/chessstrategyvstactics.html): the "pin," the "skewer," and so on. They're relatively simple; you could learn them in an afternoon. Strategy, on the other hand, relates to long-term plans and takes years or decades to master. Strategy builds upon tactics, but not mechanistically. Great players distinguish themselves by cleverly combining the core tactics and thinking (far) ahead. 

Although data analysis doesn't strongly resemble chess, the strategy/tactics distinction might still be helpful. While the long-term strategies of data analysis take years to master, they're built upon simpler core tactics. This repository aims to catalog the most useful "data tactics."

The data tactics below are roughly ordered from the simplest to the most complex.

## Summarizing Tactics

Tactics that represent, in a single number, *something* about list of numbers.

- Minimum
- Maximum
- Mean
- Median
- Mode
- Count
- Sum
- [Standard deviation](http://en.wikipedia.org/wiki/Standard_deviation)

## Pairwise Tactics

Tactics that work on a pair of numbers (or two lists of numbers).

- Subtract
- Multiply
- Divide

## Transformational Tactics

Tactics to transform individual bits of data.

- Rescale (e.g., logarithm, square root, etc.)
- Classify
- Reduce dimensions
- Extract features
- Normalize (text)
- Geocode (addresses -> lat/long)
- Resample (time series data, e.g., day -> month)
- Rolling average

## Comparative Tactics

Tactics to compare one value to a broader set of numbers.

- Rank
- Percentiles / quantiles
- Percent difference
- Z-score

## Structural Tactics

Tactics to reshape/reorganize data tables.

- Sort
- Filter/subset
- Transpose
- Join
 
## Combinatory Tactics

Tactics that combine two or more more basic tactics.

- Grouped summary statistics
- Crosstabs / pivot tables

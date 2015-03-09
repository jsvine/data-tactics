# Data Tactics

*Note: This is a half-baked work in progress.*

Chess players distinguish between [__strategy__](http://en.wikipedia.org/wiki/Chess_strategy) and [__tactics__](http://en.wikipedia.org/wiki/Chess_tactic). Strategy: long-term plans; tactics: short-term plans. Strategy requires years or decades to master; you can learn the core tactics in just a few hours or days. Strategy builds upon tactics, much like paintings build upon brushstrokes, and, perhaps, data analysis builds upon "data tactics."

Chess tactics are, essentially, [short sequences of moves](http://www.chessfornovices.com/chessstrategyvstactics.html). Likewise, "data tactics" could be thought of as short sequences of computational moves: adding all the numbers in a list, or sorting spreadsheets by a column.

The goal of this repository is to catalog the most useful data tactics, from the most basic to the more complex.

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

## Transformational Tactics

Tactics to transform individual bits of data.

- Rescale (e.g., logarithm, square root, etc.)
- Classify
- Reduce dimensions
- Extract features
- Normalize (text)
- Geocode (addresses -> lat/long)

## Combinatory Tactics

Tactics that combine two or more lists of data.

- Subtraction
- Multiplication
- Division (e.g., X per capita)

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

Google Sheets currently has 512 documented functions and several more #undocumented functions. Functions are comprised of [[Term#Primitive functions|primitive functions]], [[LAMBDA]] functions, and [[Operator|operators]]. This collection mostly deals with primitives for the sake of developing a working vocabulary of functions.

Generally speaking, most advanced users learn functions through one of two methods. The first is by by raw experience. The second, championed by [[Matt King]], involves going through the full list of functions and trying to understand each one.

This collection is meant to give a jumping-off point for learning the most common functions and is meant to be supplemented with both experience and a thorough reading of documentation.

### Basic functions

Basic functions include [[SUM]], [[AVERAGE]], and data aggregation functions in general. This is because they only take one type of argument and are generally very easy to understand, even for beginners. Since they mostly return single values, they are easy to nest.

### Intermediate functions

Intermediate functions include functions like [[VLOOKUP]], [[SORT]], and [[FILTER]]. Since these functions generally either take multiple arrays as input, return arrays as output, or have otherwise confusing syntaxes, they are typically harder to work with than basic functions. 

### Advanced functions

Advanced functions often have idiosyncratic syntax and require a significant amount of time to learn.

| Function type | Description |
| --- | --- |
| [[REGEX functions]] | Used for [[string]] processing. |
| [[QUERY]] | Used for [[table]] transformations. |
| [[LAMBDA]] | Used for abstraction and recursion. Note that [[SCAN]], [[REDUCE]], and techniques like [[LAMBDA recursion]] are all advanced, while [[BYROW]] and the like do not. |
| [[IMPORT functions]] | Used for importing data from the web. |


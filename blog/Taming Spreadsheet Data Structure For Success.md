---
author: Chris Carpenter/Aliafriend
tags:
  - tutorial
---
New spreadsheet users often struggle with data organization. We encounter data in various formats daily, but understanding its underlying structure is key. Poor data structure creates headaches later when simple tasks like analysis or filtering become cumbersome. By prioritizing a well-organized structure, even if it appears less visually appealing initially, you'll save time and frustration in the long run.

Proper data structure leads to better data ingestion, smoother experience, and easier usability.

Let's look at an example.

| A                | B             | C         |
| ---------------- | ------------- | --------- |
| Week of 4/1/2024 |               |           |
| Monday           |               |           |
|                  | Gas           | \-$25.00  |
|                  | Food          | \-$10.00  |
| Tuesday          |               |           |
|                  | Car           | \-$50.00  |
| Wednesday        |               |           |
|                  | Birthday Gift | \-$26.00  |
|                  | Food          | \-$15.00  |
| Thursday         |               |           |
|                  | Paycheck      | $400.00   |
| Friday           |               |           |
|                  | Movies        | \-$30.00  |
|                  | Candy         | \-$10.00  |
| Saturday         |               |           |
|                  | Groceries     | \-$100.00 |
| Sunday           |               |           |
|                  | Video Game    | \-$60.00  |
| Total            |               | $74.00    |
|                  |               |           |
|                  |               |           |
| Week 1           |               |           |

This is an example of a data structure that would be fine to use if you're only planning on 1-3 weeks to track expenses. However, how about 2 months, 6 months, 3 years? It becomes harder and harder to find information like "How much am i spending every week on average?" or "How much am I spending on groceries every month?"

| A        | B             | C         |
| -------- | ------------- | --------- |
| Day      | Item          | Amount    |
| 4/1/2024 | Gas           | \-$25.00  |
| 4/1/2024 | Food          | \-$10.00  |
| 4/2/2024 | Car           | \-$50.00  |
| 4/3/2024 | Birthday Gift | \-$26.00  |
| 4/3/2024 | Food          | \-$15.00  |
| 4/4/2024 | Paycheck      | $400.00   |
| 4/5/2024 | Movies        | \-$30.00  |
| 4/5/2024 | Candy         | \-$10.00  |
| 4/6/2024 | Groceries     | \-$100.00 |
| 4/7/2024 | Video Game    | \-$60.00  |
|          |               |           |
|          |               |           |
| Entries  |               |           |

While this doesn't look as nice, it's infinitely more easier to do something like

```haskell
=QUERY(A:C,"SELECT Sum(C)
 WHERE A >= date '2024-04-01' and A <= date '2024-04-07'")
```

This formula easily calculates the sum for the week or any date range you specify.

```haskell
=QUERY(A:C,"SELECT Sum(C) WHERE B ='Food'")
```

For more information see [[QUERY]]

and

```haskell
=SUM(FILTER(C:C,B:B="Food"))
```

Which would give you all the totals for how much you spent on food. You could even combine them!

This structure allows you to track weeks, months, or years and allows you to easily find the data you're looking for without looking through many sheets. It also prevents complex formulas or creating arrays of multiple different sections and changing it every week to include that week.

Let's take a look at another example.

| A      | B           | C          | D        | E        |
| ------ | ----------- | ---------- | -------- | -------- |
| PO     | Customer    | Item       | Quantity | Date     |
| 123456 | ABC Company | Water      | 1        | 4/1/2024 |
| 123456 | ABC Company | Meat       | 2        | 4/1/2024 |
| 123456 | ABC Company | Vegetables | 2        | 4/1/2024 |
| 567891 | DEF Company | Bread      | 4        | 4/3/2024 |
| 567891 | DEF Company | Salad      | 5        | 4/3/2024 |
| 234567 | ABC Company | Water      | 1        | 4/5/2024 |

While this might seem like extra work upfront, this structure allows you to easily filter by various criteria, such as specific companies or items, to see how much stock you have on hand, or other important information you may be looking for such as "How much Meat did we buy from ABC company last month?" can be answered with a simple Filter or [query](https://sheets.wiki/docs/QUERY).

By prioritizing a well-organized structure from the beginning, you'll empower yourself to get the most out of your spreadsheets!



Further information on techniques for data structure success see [[Table|tables]].
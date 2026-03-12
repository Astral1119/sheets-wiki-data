---
author: Chris Carpenter/Aliafriend
tags:
  - tutorial
  - data-organization
  - google-sheets
---
## Fixing Anti-Patterns: Merged Cells Where Data Resides

Merged cells are one of the most seductive traps in spreadsheets. They look clean and organized at first glance — perfect for titles, grouped weeks, category headings, or "pretty" reports — but when the **merged cells actually hold important data** (names, dates, values, notes), they become a nightmare for formulas. Merged cells only contain the value in the top-left most cell meaning for example FILTER() can only read the top-left most cell of a merged cell.

### Common Merged-Cell Anti-Patterns

1. **Merged row/column labels repeated across groups**  
   Example: Person names merged vertically over several rows of their transactions.

   | A          | B      | C       |
   |------------|--------|---------|
   |   Bob      | Gas    | -$25    |
   |   Merged   | Food   | -$18    |
   |   Merged   | Movies | -$12    |
   |   Sally    | Rent   | -$800   |
   |   Merged   | Food   | -$45    |
   |   Merged   | Gifts  | -$60    |

   Looks nice in a printed report… but try to:
   - Filter only Sally’s expenses
   - Sum food spending per person
   - Sort by amount, category, or person

2. **Merged headers over date groups**  
   Example: Weeks or months merged across several date columns.

   | A     | B     | C             | D     | E     | F             | G     |
   |-------|-------|---------------|-------|-------|---------------|-------|
   | Item  |       | Week of Jan 1 |       |       | Week of Jan 8 |       |
   |       | Mon   | Tue   | Wed   | Thu   | Fri   | Sat   |
   | Apples| 5     | 3     | 8     | 2     | 6     | 4     |

   You can’t easily filter by a single day, use date-based functions, or expand the table without manual labor each time.

3. **Merged cells for subtotals or notes**  
   A single merged cell spanning multiple rows/columns with a comment or total — impossible to sort, filter, or reference reliably.

**The core problem**: Merged cells violate the **tabular data rule** — every cell should contain exactly one atomic piece of information, and every row should be a complete, independent observation.

### The Fix: Unmerge + Fill Down (or Fill Right)

Once you have it back in tabular form you can create a new sheet and reference the table with the merged format that looks the way you want to. That way you will both have it look nice, yet able to do analysis that often comes with spreadsheeting.

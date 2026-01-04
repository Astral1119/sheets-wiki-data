---
tags:
  - formatting
  - conditional
---

Conditional formatting in Google Sheets applies visual formatting (colors, font styles, etc.) to cells based on their values or formulas. Understanding how conditional formatting formulas are evaluated is crucial for correct application.

### Reference Types and Their Effects

Conditional formatting formulas use cell references, and the anchor points (`$`) determine what gets compared:

| Reference | Example | Behavior |
|-----------|---------|----------|
| Fully relative | `=A1="x"` | Checks each cell against itself |
| Column-anchored | `=$A1="x"` | Checks column A of each row |
| Row-anchored | `=A$1="x"` | Checks row 1 of each column |
| Fully absolute | `=$A$1="x"` | Checks only cell A1 for all cells |

### How Formulas Are Applied

When you apply a conditional format to a range (e.g., `B2:D10`), Google Sheets evaluates the formula for **each cell** in that range, adjusting relative references accordingly:

**Example**: Format `B2:D10` with formula `=$A2="x"`
- For cell B2: checks if `$A2="x"`
- For cell B3: checks if `$A3="x"`  
- For cell C2: checks if `$A2="x"` (same as B2)
- For cell C3: checks if `$A3="x"` (same as B3)

The `$A` anchor keeps the column fixed at A, but the row number adjusts to match each cell's row.

### Common Patterns

#### Highlighting entire rows

To highlight a full row based on a single column's value:

```gse
=$A2="x"
```

Applied to range `A2:Z100`, this highlights the entire row when column A contains "x".

#### Highlighting matching cells only

To highlight only cells that contain a specific value:

```gse
=A1="x"
```

Without anchors, each cell is checked individually.

#### Avoiding false highlights on blank cells

When comparing values, blank cells can trigger unwanted highlighting. Use `AND` to exclude blanks:

```gse
=AND($B1>$C1, $B1<>"")
```

This only highlights when B1 is greater than C1 **and** B1 is not blank.

#### Highlighting based on another sheet

Reference cells on other sheets:

```gse
=Sheet2!$A1="complete"
```

### Rules for Multiple Conditions

- Multiple conditional format rules are evaluated in order (top to bottom in the rules list)
- First matching rule wins (unless "Done" is unchecked, allowing multiple rules to apply)
- More specific rules should appear before general ones

### Custom Formulas vs. Presets

Google Sheets offers preset conditions (e.g., "Greater than", "Text contains") and custom formulas. Custom formulas provide maximum flexibility but require understanding of reference anchoring.

### Performance Considerations

Complex conditional formatting formulas (especially those referencing large ranges or using heavy calculations) can slow sheet performance. Simplify formulas when possible and limit the application range.

### See Also
- [[Data type]] — understanding cell value types
- [[Array#Range]] — how ranges work with references
- [[Boolean]] — TRUE/FALSE values in conditional logic

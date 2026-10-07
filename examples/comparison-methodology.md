# Business Data Comparison Methodology

Comparing two datasets involves more than finding cells that contain different values.

A useful comparison should distinguish between different types of changes and provide enough context to investigate them.

## 1. Added records

A record exists in the current dataset but not in the previous dataset.

Example:

Webcam HD appears in `sales-current.csv` but not in `sales-previous.csv`.

This is an added record.

## 2. Removed records

A record exists in the previous dataset but no longer exists in the current dataset.

For example, if a product appears in the previous dataset but is absent from the current dataset, it can be classified as a removed record.

## 3. Changed values

A record exists in both datasets, but one or more fields have changed.

For example:

Laptop Pro:

Previous:
- Units Sold: 120
- Revenue: 144000
- Stock Quantity: 35

Current:
- Units Sold: 165
- Revenue: 198000
- Stock Quantity: 20

The product itself still exists, but multiple values changed.

## 4. Unchanged records

Some records exist in both datasets and have identical values.

These records should normally be separated from actual findings so that attention can remain on meaningful changes.

## 5. Related changes

Multiple changes can occur together.

For example, an increase in units sold combined with an increase in revenue and a decrease in stock may represent a related business event rather than three completely independent findings.

Grouping related changes can make an investigation easier to understand.

## 6. Evidence

A useful investigation should preserve the source of a finding.

Depending on the data format, evidence may include:

- File
- Sheet
- Row
- Column
- Cell
- Record
- Page
- Section

This allows a finding to be traced back to the underlying source data.

## 7. Comparison versus investigation

A basic comparison answers:

"What is different?"

An investigation attempts to answer additional questions:

- Which differences matter?
- How significant are they?
- Which changes are related?
- Where is the evidence?
- What should be investigated next?

This distinction becomes increasingly important as datasets become larger and more complex.

## QKELE

QKELE is a business data investigation and comparison platform built around these concepts.

Its deterministic comparison engine identifies additions, removals, and changed values, while the investigation workflow helps organize meaningful findings and trace them back to evidence.

AI can optionally provide advisory explanations, but the underlying comparison is based on the source data rather than AI-generated guesses.

Website: https://qkele.app

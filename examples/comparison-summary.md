# Sales Dataset Comparison Summary

This example compares `sales-previous.csv` with `sales-current.csv`.

## Findings

### Added record

Webcam HD was added to the current dataset.

Category: Electronics  
Units Sold: 140  
Revenue: 19,600  
Stock Quantity: 60

### Changed record: Laptop Pro

Units Sold:
120 → 165

Revenue:
144,000 → 198,000

Stock Quantity:
35 → 20

### Changed record: Wireless Mouse

Units Sold:
450 → 520

Revenue:
22,500 → 26,000

Stock Quantity:
120 → 95

### Changed record: 27-inch Monitor

Units Sold:
95 → 70

Revenue:
28,500 → 21,000

Stock Quantity:
40 → 55

### Unchanged records

Mechanical Keyboard and USB-C Hub have the same values in both datasets.

## Investigation observations

The Laptop Pro shows a substantial increase in units sold and revenue while its stock quantity decreased.

The 27-inch Monitor shows lower units sold and revenue while stock quantity increased.

These examples demonstrate why a comparison can be more useful when changes are presented with context rather than as an undifferentiated list of changed cells.

## Evidence

Every finding in this example can be traced to the corresponding records in:

- `examples/sales-previous.csv`
- `examples/sales-current.csv`

This illustrates an evidence-first approach to business data comparison.

## About QKELE

QKELE is a business data investigation and comparison platform that helps identify meaningful changes, connect related findings, and trace findings back to their underlying evidence.

Website: https://qkele.app

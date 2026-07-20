# Pricing and margin scenarios

This specification keeps price, tax, cost, channel charges, and contribution separate. It supports decisions without presenting internal calculations as market validation.

## Core measures

- **Net price:** selling price excluding transferred taxes.
- **Markup:** `(net price - cost) / cost`.
- **Gross margin:** `(net price - cost of sales) / net price`.
- **Contribution:** `net price - cost - included variable channel charges`.
- **Contribution margin:** `contribution / net price`.
- **Estimated result:** contribution minus explicitly configured allocations. It must not be labelled net profit when required expenses or taxes are missing.

## Cost quality

Every scenario exposes whether its cost is confirmed, estimated, incomplete, or outdated. A missing component never silently becomes a confirmed zero.

## Scenarios

- Technical floor based only on included assumptions.
- Current published price.
- Editable target.
- Promotion with channel and validity.
- Sensitivity analysis for price, cost, fees, waste, or volume.

The technical floor is not a recommendation of what the market will pay.

## Publishing lifecycle

Draft, saved scenario, scheduled, active, superseded, and voided are separate states. Saving a scenario never changes the price used by new sales. Every published change retains validity, actor, reason, and high-precision timestamp.

## Progressive interface

The pricing area appears only after a product or service exists and pricing or sales is activated. Daily use shows a compact summary; sensitivity, break-even, product mix, and history load under demand.

## Educational layer

Each measure provides contextual help, a collapsed screen glossary, and an optional technical explanation with formula, example, assumptions, limitations, and calculation inputs.

# Chiller Plant Optimisation
Cutting cooling energy in commercial buildings

## The Problem

### Cooling dominates the bill
- **60%**: of building electricity goes to cooling
- **25%**: typical savings from better controls
- **2 yrs**: usual payback
<!-- notes: Open with the scale of the problem before any technical detail. -->
<!-- doc-only -->
In hot climates, chilled-water plants run close to full load for most of the year. The table below shows a typical split.

| End use | Share | kWh/yr |
|:---|:---:|---:|
| Cooling | 60% | 3,600,000 |
| Lighting | 20% | 1,200,000 |
<!-- /doc-only -->

## The Method

### How we optimise
1. Measure
2. Model
3. Tune
4. Verify
<!-- notes: Each step is two to three weeks on a typical site. -->

### Plant efficiency
<!-- layout: cards -->
- Chillers: sequence by part-load efficiency
- Pumps: variable speed on secondary loop
- Towers: reset condenser water setpoint

$$ \eta = \frac{Q_{cool}}{P_{elec}} $$

<!-- slide-only -->
## Key Takeaways
- **Controls first**: cheapest savings
- **Meter everything**: no data, no decisions
<!-- /slide-only -->

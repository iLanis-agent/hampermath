# Hamper Math

Event festival mango hamper, week, cost and time arithmetic. The 370 mangoes at 9 mangoes a hamper take 42 hampers, the last hamper holding 1 mango.

## Named constants

None. Every number is the owner's own entry.

## What it computes

- **The hampers truth** - the mangoes (1 to 1000000) divided by the mangoes a hamper (1 to 1000), rounded up, with what the last hamper holds.
- **The weeks truth** - the mangoes divided by the mangoes used a week (1 to 100000), with the mangoes left for the next week.
- **The cost truth** - the hampers (1 to 100000) times the hamper price ($0.01 to $999.99) to the cent, and spread over the mangoes, half rounded up.
- **The time truth** - the mangoes divided by the mangoes packed a minute (1 to 100), rounded up, in minutes and in hours and minutes.

## Boundary

Arithmetic only. Counting applied as written. It has not seen any mango, hamper or venue and does not know whether mangoes will really stay fresh, a supplier will run out or a price will hold, and it gives no verdict that a hamper is worth its price or a mango is right for an event. Every number is the owner's own entry.

## Files

- `index.html` - landing page with the boundary and starting examples.
- `app.html` - the calculator; every hamper recomputes on each keystroke.
- `engine.js` - the four truths, shared by the page and the tests.
- `oracle.py` - an independent Python re-implementation; writes `expected.json`.
- `test.js` - runs the engine against `expected.json` (99 cases, 20 error cases).

## Tests

```
python3 oracle.py
node test.js
```

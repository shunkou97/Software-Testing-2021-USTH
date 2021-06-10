### *Question*

**Write the predicate (only the predicate) to represent the requirement:**

“List all the wireless mice that either retail for more than $100 or for which the store has more than 20 items. Also list non-wireless mice that retail for more than $50.”

### *Answer*

```
((MouseType = Wireless) ∧ ((Retail > 100) ∨ (Stock > 20))) ∨ (¬(MouseType = Wireless) ∧ (Retail > 50))
```

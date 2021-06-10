#### Characteristic: Location of element in list
```  
  Block 1: Element is first entry in list.
  Block 2: Element is last entry in list.
  Block 3: Element is in some position other than first or last.
```

a) *“Location of element in list” fails the disjointness property. **Give an example that illustrates this**.*
    
    If there is only 1 element in the list, block 1 and 2 will be jointed thus violates the disjointness property.
 
b) *“Location of element in list” fails the completeness property. **Give an example that illustrates this**.*

    If the element is null or not in the list, thus fails the completeness property.
    
c) *Supply **one or more new partitions** that capture the intent of “Location of element in list” but do not suffer from completeness or disjointness problems.*

    Block 1: Element is null.
    Block 2: Element is not null but not in the list.

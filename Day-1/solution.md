## Event Scheduling Problem

### Objective:
Minimize the number of rooms used.

### Sets:
- \( V \): Set of events (vertices).
- \( E \): Set of edges where \( (u, v) \in E \) indicates events \( u \) and \( v \) have overlapping participants.

### Parameters:
- \( n \): Number of events.

### Variables:
- \( x_{i,k} \): Binary variable, equals 1 if event \( i \) is assigned to room \( k \), and 0 otherwise.
- \( R \): Total number of rooms used.

### Formulation:
**Objective Function:**

Minimize \( R \)

**Subject to:**

1. Each event must be assigned to exactly one room:
   $$ \sum_{k=1}^n a_k b_k = \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right) $$

2. No two overlapping events can be assigned to the same room:
   $$ \sum_{k=1}^n a_k b_k = \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right) $$

3. Define the total number of rooms used:
   $$ \sum_{k=1}^n a_k b_k = \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right) $$




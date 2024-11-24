# Project Overview
Design the least-cost transmission system additions to integrate 75 MW of utility solar PV while resolving existing system reliability issues.

## Core Requirements
1. Power Integration
   - 75 MW solar PV plant at NEWSOLAR substation
   - Currently has 69-kV bus (NEWSOLAR69, bus 60)
   - Solar modeled as PV bus with ±35 Mvar reactive power limits
   - Must function with solar at both full capacity and offline

2. Reliability Requirements
   - Two separate transmission lines to NEWSOLAR required
   - No violations during normal operation
   - No violations during N-1 contingencies
   - Voltage limits: 0.95 - 1.10 per unit
   - Line flows: ≤100% of limit A values

3. Infrastructure Options
   - NEWSOLAR substation can accommodate 138-kV bus and 138/69-kV transformer
   - All existing 69-kV substations can be upgraded to 138-kV
   - All existing buses can accept new transmission lines

## Available Equipment & Costs

### Transmission Lines
1. Fixed Costs:
   - 138-kV line: $1,250,000
   - 69-kV line: $750,000

2. Conductor Options & Variable Costs ($/km):
   - Rook (770A): 138kV = $370,000/km
   - Crow (830A): 138kV = $500,000/km, 69kV = $390,000/km
   - Condor (900A): 138kV = $525,000/km, 69kV = $410,000/km
   - Cardinal (1110A): 138kV = $540,000/km

3. Available Rights-of-Way:
   - NEWSOLAR to: OAK (13km), BUCKEY (6km), APPLE (6km), PINE (14km), MAPLE (15km)
   - Other routes: 
     * BUCKEYE-OAK: 8km
     * BUCKEYE-ORANGE: 8km
     * APPLE-PINE: 10km
     * APPLE-ORANGE: 9km
     * APPLE-LOCUST: 10km

### Transformers & Substations
1. Transformer Options:
   - 138/69 kV, 101 MVA: $1,500,000
   - 138/69 kV, 168 MVA: $1,800,000

2. Substation Upgrades:
   - Cost to add 138kV to existing 69kV substation: $900,000

## Economic Considerations
- Calculate 5-year loss reduction benefits
- Electricity priced at $60/MWh
- Total cost = Construction costs - Loss reduction savings

## Simplifying Assumptions
1. Consider only base case loading level
2. Existing generator outputs are fixed (changes via slack bus only)
3. No modification of capacitors or transformer taps
4. System losses remain constant over 5-year period
5. Only consider base case loss impacts

## Design Process Requirements
1. Start with PowerWorld case Chapter6_Design1Start
2. Analyze base case operation
3. Perform contingency analysis
4. Design least-cost additions meeting all requirements
5. Document justification for final recommendation

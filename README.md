# Trav

A few automation scripts to make Traveler RPG game play a little more streamlined.

**Note:** All scripts have a help section that is visible by appending ```--help``` to the end of any command. e.g. ```trav --help``` will list trav scripts ```trav passengers --help``` will show help for the passengers script.


## Available Scripts

### Calculate Availiable Passengers

**Command:**
```
./trav passengers --current "Agricultural, Rich" --destination "Water world, Rich" --dm 2 --staterooms 10 --low-berths 20
```

**Output:**
```
Streetwise/Carouse Check (2d6 + 2):
|-> Roll:5
|-> Calculated Effect: -3

World Modifiers:
|-> Current:
| |-> Agricultural: 0
| |-> Rich: -1
| |-> TOTAL: -1
|
|-> Destination:
| |-> Water world: 0
| |-> Rich: 2
| |-> TOTAL: 2

Total Modifiers:
|-> Effect Modifier (half of effect): -2
|-> Current World Modifier: -1
|-> Destination World Modifier: 2
|-> TOTAL: 2

Availiable Passengers:
|-> High: 0
|-> Medium: 0
|-> Low Berth: 0

Passenger Optimization:
|-> High Passengers: 0 * 6000 = 0 CR
|-> Medium Passengers: 0 * 3000 = 0 CR
|-> Low Berth Passengers: 0 * 1000 = 0 CR
|-> TOTAL INCOME: 0 CR
```

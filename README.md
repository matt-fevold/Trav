# Trav

A few automation scripts to make Traveler RPG game play a little more streamlined. The scripts should try to remain reletively transparent where scores are coming from so that they can be validated manually, step-by-step.

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

**Command:**
```
./trav passengers --current "Agricultural" --destination "Water world, Rich" --dm 2 --staterooms 10 --low-berths 20 
```

**Output:**
```
Streetwise/Carouse Check (2d6 + 2):
|-> Roll:8
|-> Calculated Effect: 0

World Modifiers:
|-> Current:
| |-> Agricultural: 0
| |-> TOTAL: 0
|
|-> Destination:
| |-> Water world: 0
| |-> Rich: 2
| |-> TOTAL: 2

Total Modifiers:
|-> Effect Modifier (half of effect): 0
|-> Current World Modifier: 0
|-> Destination World Modifier: 2
|-> TOTAL: 2

Availiable Passengers:
|-> High: 1
|-> Medium: 1
|-> Low Berth: 9

Passenger Optimization:
|-> High Passengers: 1 * 6000 = 6000 CR
|-> Medium Passengers: 1 * 3000 = 3000 CR
|-> Low Berth Passengers: 9 * 1000 = 9000 CR
|-> TOTAL INCOME: 18000 CR
```

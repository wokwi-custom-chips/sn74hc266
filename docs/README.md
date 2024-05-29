# Wokwi sn74hc266 Chip

This is a custom chip for [Wokwi](https://wokwi.com/). It implements a  faur independent 2-INPUT exclusive-NOR gates in Positive logic . The chip performs the following boolean function :  Y = NOT( A . B) + (A . B) 
## Truth Table 
|  INPUT A |  INPUT B | OUTPUTS  |
| ------- | ------- | -------- |
|    L    |    L    |     H    |
|    L    |    H    |     L    |
|    H    |    L    |     L    | 
|    H    |    H    |     H    | 


## Pin names

| Name  | Description              |
| ----  | ------------------------ |
| 1A    | Gate 1 Input signal  A   |
| 1B    | Gate 1 Input signal  B   |
| 1Y    | Gate 1 Output signal     |
| 2A    | Gate 2 Input signal  A   |
| 2B    | Gate 2 Input signal  B   |
| 2Y    | Gate 2 Output signal     |
| 3A    | Gate 3 Input signal  A   |
| 3B    | Gate 3 Input signal  B   |
| 3Y    | Gate 3 Output signal     |
| 4A    | Gate 4 Input signal  A   |
| 4B    | Gate 4 Input signal  B   |
| 4Y    | Gate 4 Output signal     |
| GND   | Ground                   |
| VCC   | Supply voltage           |

## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-sn74hc266": "github:wokwi-custom-chips/sn74hc266@0.1.0"
  }
```

Then, add the chip to your circuit by adding a `chip-sn74hc266` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "chip-sn74hc266", "id": "chip1" }
  },
```

For a complete example, see [the sn74hc266 chip test project](https://wokwi.com/projects/398979524422866945).

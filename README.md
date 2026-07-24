# TIA-portal-two-hand-safety-interlock
Same safety interlock i made for Arduino Opta but remade in TIA portal

## Ladder Logic Overview
![Two-Hand Safety Logic](logic_diagram.png)

## Hardware Allocation

| Variable Name | Address | Type | Function |
| :--- | :--- | :--- | :--- |
| `button1` | `%I0.0` | BOOL | Left Hand Push Button |
| `button2` | `%I0.1` | BOOL | Right Hand Push Button |
| `limit_switch` | `%I0.2` | BOOL | Position Feedback / Interlock |
| `reset` | `%I0.3` | BOOL | Reset Push Button |
| `green` | `%Q0.0` | BOOL | Run Signal Output |
| `red` | `%Q0.1` | BOOL | Error Signal Output |
| `yellow` | `%Q0.2` | BOOL | Standby Signal Output |

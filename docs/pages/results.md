> [!NOTE]
> Some information is deliberately omitted. We will be publishing the full details once our research paper is published.

## Frameworks Under Test
- Things Hive
- Bare-metal C
- Lua
- Python
- mRuby
- uPython

## Applications Under Test
The following applications are developed for each framework, then the performance is analyzed and compared with Hive:
- Print
- Temperature Monitor
- n<sup>th</sup> Harmonic Series

## Run-Time Analysis

### Print Application
```charty
{
    "title":   "Bare-Metal C",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Static", "value": 1.24 },
        { "label": "Dynamic", "value": 1 }
    ]
}
```
```charty
{
    "title":   "HIVE",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Static", "value": 13.73 },
        { "label": "Dynamic", "value": 1.16 }
    ]
}
```
```charty
{
    "title":   "Lua",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Static", "value": 166.17 },
        { "label": "Dynamic", "value": 43.50 }
    ]
}
```
```charty
{
    "title":   "mRuby",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Static", "value": 693.94 },
        { "label": "Dynamic", "value": 112.31 }
    ]
}
```
```charty
{
    "title":   "microPython",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Static", "value": 4248.99 },
        { "label": "Dynamic", "value": 360.91 }
    ]
}
```
```charty
{
    "title":   "Python3",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Static", "value": 304.97 },
        { "label": "Dynamic", "value": 21.4 }
    ]
}
```
## Footprint Analysis

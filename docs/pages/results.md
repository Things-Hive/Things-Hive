> [!NOTE]
> Some information is deliberately omitted. We will be releasing the full details once our research paper is published.

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
  - This application simply prints the message "Hello From The Queen!!!".
- Temperature Monitor
  - This application represents a simple IoT application loop. Communicates with a temperature sensor over I2C, converts the binary number into decimal Celsius representation, prints the value to the console, and displays the temperature value on an I2C-based 7-segment display. 
- n<sup>th</sup> Harmonic Series
  - Calculates the 100,000,000th harmonic number in the harmonic series. This application is used to evaluate the performance of HIVE in looping, branching, and large amounts of float data computation.

Each application was executed 100 times, and the results recorded and displayed as follows.

## Execution-Time Analysis
All values are in seconds.
```charty
{
    "title":   "Print",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 0.0465 },
        { "label": "uPython - ", "value": 0.0259 },
        { "label": "mRuby - ", "value": 0.0127 },
        { "label": "Lua - ", "value": 0.0108 },
        { "label": "C - ", "value": 0.01 },
        { "label": "HIVE - ", "value": 0.0101 }
    ]
}
```

```charty
{
    "title":   "Temperature",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 0.0465 },
        { "label": "uPython - ", "value": 0.0275 },
        { "label": "mRuby - ", "value": 0.0140 },
        { "label": "Lua - ", "value": 0.0122 },
        { "label": "C - ", "value": 0.0111 },
        { "label": "HIVE - ", "value": 0.0112 }
    ]
}
```

```charty
{
    "title":   "Harmonics",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 27.42 },
        { "label": "uPython - ", "value": 46.14 },
        { "label": "mRuby - ", "value": 53.64 },
        { "label": "Lua - ", "value": 14.24 },
        { "label": "C - ", "value": 1.08 },
        { "label": "HIVE - ", "value": 10.22 }
    ]
}
```

## Static Memory Analysis
All values are in KBs.
```charty
{
    "title":   "Print",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 4248.99 },
        { "label": "uPython - ", "value": 304.97 },
        { "label": "mRuby - ", "value": 693.94 },
        { "label": "Lua - ", "value": 125.76 },
        { "label": "C - ", "value": 1.24 },
        { "label": "HIVE - ", "value": 13.73 }
    ]
}
```

```charty
{
    "title":   "Temperature",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 4248.99 },
        { "label": "uPython - ", "value": 304.97 },
        { "label": "mRuby - ", "value": 693.94 },
        { "label": "Lua - ", "value": 125.76 },
        { "label": "C - ", "value": 1.54 },
        { "label": "HIVE - ", "value": 14.42 }
    ]
}
```

```charty
{
    "title":   "Harmonics",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 4248.99 },
        { "label": "uPython - ", "value": 304.97 },
        { "label": "mRuby - ", "value": 693.94 },
        { "label": "Lua - ", "value": 125.76 },
        { "label": "C - ", "value": 1.36 },
        { "label": "HIVE - ", "value": 13.97 }
    ]
}
```

## Dynamic Memory Analysis
All values are in KBs.
```charty
{
    "title":   "Print",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 365.48 },
        { "label": "uPython - ", "value": 29.10 },
        { "label": "mRuby - ", "value": 132.97 },
        { "label": "Lua - ", "value": 68.77 },
        { "label": "C - ", "value": 1.34 },
        { "label": "HIVE - ", "value": 3.52 }
    ]
}
```

```charty
{
    "title":   "Temperature",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 365.48 },
        { "label": "uPython - ", "value": 29.10 },
        { "label": "mRuby - ", "value": 132.97 },
        { "label": "Lua - ", "value": 68.77 },
        { "label": "C - ", "value": 1.34 },
        { "label": "HIVE - ", "value": 3.52 }
    ]
}
```

```charty
{
    "title":   "Harmonics",
    "type":    "pie",
    "options": {
        "legend":  true,
        "labels":  true,
        "numbers": true
    },
    "data": [
        { "label": "Python 3 - ", "value": 360.91 },
        { "label": "uPython - ", "value": 1028.02 },
        { "label": "mRuby - ", "value": 205.27 },
        { "label": "Lua - ", "value": 24.63 },
        { "label": "C - ", "value": 1.00 },
        { "label": "HIVE - ", "value": 1.39 }
    ]
}
```


[comment]: <> (### Print Application)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Bare-Metal C",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 1.24 },)

[comment]: <> (        { "label": "Dynamic", "value": 1 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "HIVE",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 13.73 },)

[comment]: <> (        { "label": "Dynamic", "value": 1.16 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Lua",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 125.76 },)

[comment]: <> (        { "label": "Dynamic", "value": 23.50 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "mRuby",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 693.94 },)

[comment]: <> (        { "label": "Dynamic", "value": 112.31 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "microPython",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 304.97 },)

[comment]: <> (        { "label": "Dynamic", "value": 1.43 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Python3",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 4248.99 },)

[comment]: <> (        { "label": "Dynamic", "value": 360.91 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)


[comment]: <> (### Temperature Application)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Bare-Metal C",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 1.54 },)

[comment]: <> (        { "label": "Dynamic", "value": 1.34 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "HIVE",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 14.42 },)

[comment]: <> (        { "label": "Dynamic", "value": 3.52 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Lua",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 125.76 },)

[comment]: <> (        { "label": "Dynamic", "value": 68.77 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "mRuby",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 693.94 },)

[comment]: <> (        { "label": "Dynamic", "value": 132.97 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "microPython",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 304.97 },)

[comment]: <> (        { "label": "Dynamic", "value": 29.10 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Python3",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 4248.99 },)

[comment]: <> (        { "label": "Dynamic", "value": 365.48 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)


[comment]: <> (### Harmonics Application)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Bare-Metal C",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 1.36 },)

[comment]: <> (        { "label": "Dynamic", "value": 1.00 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "HIVE",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 13.97 },)

[comment]: <> (        { "label": "Dynamic", "value": 1.39 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Lua",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 125.76 },)

[comment]: <> (        { "label": "Dynamic", "value": 24.63 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "mRuby",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 693.94 },)

[comment]: <> (        { "label": "Dynamic", "value": 205.27 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "microPython",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 304.97 },)

[comment]: <> (        { "label": "Dynamic", "value": 1028.02 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

[comment]: <> (```charty)

[comment]: <> ({)

[comment]: <> (    "title":   "Python3",)

[comment]: <> (    "type":    "pie",)

[comment]: <> (    "options": {)

[comment]: <> (        "legend":  true,)

[comment]: <> (        "labels":  true,)

[comment]: <> (        "numbers": true)

[comment]: <> (    },)

[comment]: <> (    "data": [)

[comment]: <> (        { "label": "Static", "value": 4248.99 },)

[comment]: <> (        { "label": "Dynamic", "value": 360.91 })

[comment]: <> (    ])

[comment]: <> (})

[comment]: <> (```)

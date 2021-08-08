# Styles

## Note Callout
> [!NOTE|style:callout]
> Test

## Note Flat
> [!NOTE]
> Test

## Tip Flat
> [!TIP]
> Test

## Warning Flat
> [!WARNING]
> Test

## Attention Flat
> [!ATTENTION]
> Test

## Comment Custom Flat
> [!COMMENT|iconVisibility:hidden]
> An alert of type 'tip' using alert specific style 'flat' which overrides global style 'callout'.
> In addition, this alert uses an own heading and hides specific icon.

## Material Icons
:mi md-18|home:
:mi-outlined red|check_circle:
:mi-round md-36 blue|check_circle:
:mi-two-tone md-48 green-svg|check_circle:
:mi-two-tone md-48 blue-svg|chrome_reader_mode:
:mi-sharp green-svg md-48|chrome_reader_mode:

!> **Important** notice with `inline code` and additional placeholder text used
to force the content to wrap and span multiple lines.

?> **Tip** notice with `inline code` and additional placeholder text used to
force the content to wrap and span multiple lines.

This is `inline code`

```javascript
const add   = (num1, num2) => num1 + num2;
const total = add(1, 2);

console.log(total); // 3
```

```html
<body>
    <p>Hello</p>
</body>
```

<!-- tabs:start -->

#### **English**

Hello!

#### **French**

Bonjour!

#### **Italian**

Ciao!

<!-- tabs:end -->

## Charts

```charty
{
  "title":   "Print Footprint",
  "caption": "With a caption",
  "type":    "radar",
  "options": {
	"legend":  true,
    "labels":  true,
    "numbers": true
  },
  "data": [
    {
		"label": "iPhone",
		"value": [64, 23, 45, 34, 52, 43, 59, 40],
		"points": [
			"Features",
			"Style",
			"Usability",
			"Ratings",
			"Apps",
			"Softness",
			"Ruggedness",
			"Appeal"
		]
	},
	{
		"label": "Android",
		"value": [86, 53, 55, 66, 80, 46, 49, 40]
	},
	{
		"label": "Chrome",
		"value": [100, 35, 76, 90, 36, 9, 0, 90]
	}
  ]
}
```

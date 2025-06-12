# Browser Source Timer for OBS

A customizable countdown/countup timer designed for use as a browser source in OBS Studio.

## Features

- Countdown and countup functionality
- Customizable colors, fonts, and sizes
- Loop option for repeating timers
- Transparent background support
- Google Fonts integration
- URL parameter configuration

## GitHub Pages Setup

1. Fork or clone this repository
2. Go to your repository settings
3. Navigate to "Pages" section
4. Select "Deploy from a branch" as source
5. Choose "main" branch and "/ (root)" folder
6. Save the settings

Your timer will be available at: `https://yourusername.github.io/browser-source-timer/`

## Usage in OBS

1. Add a new "Browser Source" in OBS
2. Use the timer URL with parameters:
   ```
   https://yourusername.github.io/browser-source-timer/timer.html?parameters
   ```

## URL Parameters

| Parameter | Description | Example |
|-----------|-------------|---------|
| `time` | Duration in seconds | `7500` (2h 5m) |
| `colour` | Text color (hex without #) | `414141` |
| `size` | Font size in pixels | `248` |
| `background` | Background color (hex without # or "transparent") | `transparent` |
| `radius` | Border radius in pixels | `0` |
| `font` | Google Font name (use + for spaces) | `Anton` |
| `direction` | Timer direction | `CountDown` or `CountUp` |
| `loop` | Loop when finished | `true` or `false` |

## Example URLs

### Countdown Timer
```
timer.html?time=7500&colour=414141&size=248&background=transparent&radius=0&font=Anton&direction=CountDown&loop=false
```

### Countup Timer
```
timer.html?time=3600&colour=ff0000&size=200&background=000000&radius=10&font=Roboto&direction=CountUp&loop=true
```

## Local Testing

You can test the timer locally by opening `timer.html` in your browser with the desired parameters.

## Troubleshooting

- Make sure all parameters are properly URL encoded
- For transparent backgrounds, use `background=transparent`
- Font names with spaces should use `+` (e.g., `Open+Sans`)
- Colors should be hex values without the `#` symbol

## License

This project is open source and available under the MIT License.
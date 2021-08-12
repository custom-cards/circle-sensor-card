# Circle Sensor Card

![Circle Sensor Examples](circle-sensor.png)

Custom component for lovelace which can be used as a card or an element on a picture-elements card.

## Installation
Add to resources:
```yaml
resources:
  - url: /hacsfiles/circle-sensor-card/circle-sensor-card.js
    type: module
```

## Example
Full documentation available in the [repository](https://github.com/custom-cards/circle-sensor-card)
```yaml
- type: custom:circle-sensor-card
  entity: sensor.outside_temperature
  max: 120
  min: 30
  stroke_width: 10
  gradient: true
  units: ' '
  attribute: 'ambient'
  attribute_max: 'feels_like'
  show_max: true
  font_style:
    color: red
    font-size: 1.5em
    text-shadow: '2px 2px black'
    font-family: 'Trebuchet MS'
  color_stops:
    50: '#55FF55'
    75: '#5555FF'
    100: '#FF5555'
  style:
    top: 50%
    left: 50%
    width: 75px
    height: 75px
```

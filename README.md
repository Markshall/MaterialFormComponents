# Material Form Components
A few basic web-form components styled with inspiration from the Google Material design language.

Each component has a various set of sizes (standard/medium/large) and can also use the same colour scheme as other components.

This library is wrote in Sass but the compiled CSS document is still available in this repository.

## Features
* Checkboxes
* Pill-styled checkboxes
* Radio buttons
* Buttons
* Text fields

## Colours
* Red (#f44336)
* Green (#56da97)
* Blue (#2196f3)
* Orange (#ff9800)
* Pink (#e91e63)
* Yellow (#fdd835)
* Brown (#795548)
* Grey (#9e9e9e)
* Purple (#673ab7)

## Previews

### Checkboxes
#### Unchecked
![Unchecked checkboxes](assets/checkbox-unchecked.PNG)
#### Checked
![Checked checkboxes](assets/checkbox-checked.PNG)
#### Various sizes
![Checkbox sizes](assets/checkbox-sizes.PNG)

### Pill checkboxes
#### Unchecked
![Unchecked pill checkboxes](assets/pill-unchecked.PNG)
#### Checked
![Checked pill checkboxes](assets/pill-checked.PNG)
#### Various sizes
![Pill checkbox sizes](assets/pill-sizes.PNG)

### Radio buttons
#### Unchecked
![Unhecked radio button](assets/radio-unchecked.PNG)
#### Checked
![Checked radio button](assets/radio-checked.PNG)
#### Various sizes
![Radio button sizes](assets/radio-sizes.PNG)

### Buttons
#### Normal state
![Normal state buttons](assets/button-normal.PNG)
#### Various sizes
![Button sizes](assets/button-sizes.PNG)

### Text fields
#### Normal state
![Normal state text field](assets/textfield-normal.PNG)
#### Focused state
![Focused state text field](assets/textfield-focused.PNG)

## Usage
If you don't want to use a coloured component, just omit the `input--x` class from the class list of your element, where `x` is a colour name.
If your element is single-lined, you add the colour to the element itself, if it contains a wrapping `div`, you must attach the colour to that.

Different sizes can be applied by adding `medium` or `large` to the same class list as your component colour. For example: `<div class="checkbox input--red medium">` or `<input type="radio" class="radio input--pink large" />`

To disable an element, just add the HTML attribute `disabled` to the form element and it will disable the rest of the styling. It applies an alpha-transparency of 0.4 and sets a 'not-allowed' cursor upon hover.

### Checkboxes
```html
<div class="checkbox input--red">
  <input type="checkbox" />
  <div class="checkbox-tick"></div>
</div>
```

### Pill checkboxes
```html
<div class="pill-checkbox input--green">
  <input type="checkbox" />
  <div class="pill-checkbox--toggle"></div>
</div>
```

### Radio buttons
```html
<input type="radio" class="radio input--blue" />
```

### Buttons
```html
<button type="button" class="button input--brown" />
```

### Text fields
```html
<div class="textfield-wrapper input--orange">
  <input type="text" class="textfield" />
  <div class="textfield-bar"></div>
</div>
```
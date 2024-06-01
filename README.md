A CSS library that provides a variety of Pokemon type icons.
![gen8](https://github.com/Fortelle/pokemon-type-css/assets/38492315/2f0b435d-7114-4fac-bf5c-ebc3c9dd0ad0)
![gen9](https://github.com/Fortelle/pokemon-type-css/assets/38492315/88b8aabb-8df4-4e24-bc2f-935259385165)

## Getting started
It's easy to create a type icon by using an inline HTML tag(commonly ```<i>``` or ```<span>```) with a layout class(```.pt-icon```, ```pt-label```...) and a type class(```pt-type-grass```, ```pt-type-fire```...).

```html
<i class="pt-icon pt-type-normal"></i>
```

In additional, you can use ```pt-icon-gen*``` classes to change the variation, and ```.pt-color-*``` classes to change the color scheme.

## Layouts
### Icons
| Classes | Preview
| - | - 
| ```.pt-icon``` | ![pt-icon](https://github.com/Fortelle/pokemon-type-css/assets/38492315/40290e51-e167-447c-bb11-ff4478f0890c)
| ```.pt-icon.pt-icon-squared``` | ![pt-icon-squared](https://github.com/Fortelle/pokemon-type-css/assets/38492315/5ee03464-e5ab-4d64-aea5-098d79d5241d)
| ```.pt-icon.pt-icon-rounded```| ![pt-icon-rounded](https://github.com/Fortelle/pokemon-type-css/assets/38492315/e9326bba-fba6-4456-a715-a887bc4b5482)

### Labels
| Classes | Preview
| - | - 
| ```.pt-label.pt-label-sm```| ![pt-label-sm](https://github.com/Fortelle/pokemon-type-css/assets/38492315/47231568-2a33-4de6-a76c-88b04aa38257)
| ```.pt-label.pt-label-swsh``` | ![pt-label-swsh](https://github.com/Fortelle/pokemon-type-css/assets/38492315/32c37bd8-62af-4f6a-aa77-ccc05c3e20b5)
| ```.pt-label.pt-label-la``` | ![pt-label-la](https://github.com/Fortelle/pokemon-type-css/assets/38492315/d42327e1-e0b8-44bb-bea3-d7cd959b8bb5)
| ```.pt-label.pt-label-bdsp```| ![pt-label-bdsp](https://github.com/Fortelle/pokemon-type-css/assets/38492315/5ee716a7-2641-41b0-ab60-66b8f093b34b)
| ```.pt-label.pt-label-sv```| ![pt-label-sv](https://github.com/Fortelle/pokemon-type-css/assets/38492315/8503b9e1-3387-4625-b061-560b6f59ae05)

### Text
```html
Bulbasaur is both <span class="pt-text pt-type-grass">Grass</span> and <span class="pt-text pt-type-poison">Poison</span> type.
```
![pt-text](https://github.com/Fortelle/pokemon-type-css/assets/38492315/8884e0eb-487d-40fc-9f84-5e371b377066)

## Modifiers
The modifier classes can be set on the icon element, or any of its ancestor elements.

The following two codes provide the same result.
```html
<div>
    <i class="pt-icon pt-icon-gen9 pt-color-sv pt-type-grass"></i>
    <i class="pt-icon pt-icon-gen9 pt-color-sv pt-type-fire"></i>
    <i class="pt-icon pt-icon-gen9 pt-color-sv pt-type-water"></i>
    <i class="pt-icon pt-icon-gen9 pt-color-sv pt-type-electric"></i>
</div>
```
```html
<div class="pt-icon-gen9 pt-color-sv">
    <i class="pt-icon pt-type-grass"></i>
    <i class="pt-icon pt-type-fire"></i>
    <i class="pt-icon pt-type-water"></i>
    <i class="pt-icon pt-type-electric"></i>
</div>
```
![pt-icon](https://github.com/Fortelle/pokemon-type-css/assets/38492315/5b1e74b2-d765-4a44-adb7-d2f3d0ab6a6b)

### Variations
- ```pt-icon-gen8```
- ```pt-icon-gen9```

### Colors
- ```pt-color-sm```
- ```pt-color-swsh```
- ```pt-color-bdsp```
- ```pt-color-la```
- ```pt-color-sv```

### Languages
- ```pt-lang-chs```
- ```pt-lang-cht```
- ```pt-lang-eng```
- ```pt-lang-fra```
- ```pt-lang-ger```
- ```pt-lang-ita```
- ```pt-lang-jpn```
- ```pt-lang-kor```
- ```pt-lang-spa```

## Customization
### Sizing
The size of an icon is based on its font size.

Icon elements can be scaled by adjusting either the ```font-size``` or the ```width``` property.
If both properties are set, the ```width``` takes precedence.

Label elements can be scaled by adjusting the ```font-size``` property.
Simply changing the ```width``` will not affect the size of the text.
If you do it, you have to change the text size manually.

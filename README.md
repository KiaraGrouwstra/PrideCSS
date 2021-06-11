## PrideCSS, a BEM-compliant SCSS library for adding pride flags

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/VKEA/PrideCSS/issues)
[![Build Status](https://travis-ci.com/VKEA/PrideCSS.svg?branch=master)](https://travis-ci.com/VKEA/PrideCSS)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/2543248deaf74fab817ff52cabc1ee84)](https://www.codacy.com/gh/VKEA/PrideCSS/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=VKEA/PrideCSS&amp;utm_campaign=Badge_Grade)
[![Known Vulnerabilities](https://snyk.io/test/github/VKEA/PrideCSS/badge.svg)](https://snyk.io/test/github/VKEA/PrideCSS?targetFile=package.json)

PrideCSS is a SCSS library for adding pride flags to your HTML elements.

SCSS source can be found in the `scss`folder, compiled CSS can be found inside the`css` folder.

## Usage

PrideCSS class names start with the word `pride`, followed by Block Element Modifier (BEM) modifiers.

Example

```html
<div class="pride--nb"></div>
```

You can use different modifiers like `horizontal`, `radial` or `bottomleft` to specify the direction of the pride gradient.

Examples

```html
<div class="pride--radial--lesbian"></div>
<div class="pride--horizontal--gay"></div>
<div class="pride--topright--ace"></div>
```

## Modifiers

### Pride flags

| Flag           | Type     |
|----------------|---------:|
| agender        | standard |
| agender2       | standard |
| androgyne      | standard |
| androgyne2     | standard |
| aro            | standard |
| aro2           | standard |
| aro3           | standard |
| ace            | standard |
| bear           | standard |
| bi             | standard |
| demiboy        | standard |
| demigender     | standard |
| demigirl       | standard |
| demisexual     | complex  |
| gay            | standard |
| genderfluid    | standard |
| genderqueer    | standard |
| gilbertbaker   | standard |
| intersex       | radial   |
| intersex2      | standard |
| lesbian        | standard |
| lesbian2       | standard |
| lesbian3       | standard |
| maverique      | standard |
| mlm            | standard |
| mlm2           | standard |
| mlm3           | standard |
| neutrois       | standard |
| nb             | standard |
| nb2            | standard |
| nb3            | standard |
| pan            | standard |
| philadelphia   | standard |
| polygender     | standard |
| polysexual     | standard |
| sapphic        | standard |
| trans          | standard |
| twink          | standard |

### Gradient directions
| Direction                   | Compatibility             |
|-----------------------------|--------------------------:|
| {name}                      | standard, radial, complex |
| horizontal--{name}          | standard                  |
| topleft--{name}             | standard                  |
| topright--{name}            | standard                  |
| bottomright--{name}         | standard                  |
| bottomleft--{name}          | standard                  |
| radial--{name}              | standard, radial          |
| radial--top--{name}         | standard, radial          |
| radial--bottom--{name}      | standard, radial          |
| radial--left--{name}        | standard, radial          |
| radial--right--{name}       | standard, radial          |
| radial--topleft--{name}     | standard, radial          |
| radial--topright--{name}    | standard, radial          |
| radial--bottomright--{name} | standard, radial          |
| radial--bottomleft--{name}  | standard, radial          |
| border--thin--{name}        | standard                  |
| border--thin--{name}        | standard                  |
| border--thick--{name}       | standard                  |
| border--dummythicc--{name}  | standard                  |

## CDN

This is on a personal site, not ideal, but it's something:
<https://ztfreak.kho.nu/pridecss/releases/2.1.css>

## Contributing

Flags and CSS generation are split. `_flags.scss` is where the flags are defined, `pride.scss` and `pride-lite.scss` use the flags to generate CSS.

Run `npm i` to install Grunt, SCSS and Stylelint packages.

If you have the Grunt CLI, you can run `grunt`, which automatically compiles and lints your changes.

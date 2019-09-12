## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Content](#content)
* [Workflows](#workflows)
* [Setup](#setup)
* [Status](#status)

## General info
This project started as a simple sketch helper library for a responsive browser bar that can be used in design mock-ups. It soon started serving another purpose for demonstrating a scalable sketch library set up, as it further separates the components of the browser bar into dedicated libraries.
	
## Technologies
Project is created with:
* Sketch version: 57.1

## Content

### Colors

`libs/library-colors.sketch`

<img src="img/library-colors.jpg" width="390" height="230"/>

All the design elements are derived from and link back to the color palette. Making changes here will affect elements in every `.sketch` file belonging to this project, with the exception of fonts. Building everything with nested color symbols ensures full color consistency, makes it possible to update brand colors from a single source and helps creating themes derived from the same palette using symbol overrides.

---

### Icons

`libs/library-icons.sketch`

<img src="img/library-icons.jpg" width="516" height="82"/>

Icons are shapes masking color symbols. This file makes no assumptions on color usage within real context and therefore all the icons default to black. Icons that use more than one color are constructed out of as many dedicated shapes as there are needed colors.

---

### Fonts

`libs/library-font-system.sketch`

<img src="img/fonts-white.jpg" width="840" height="213"/>

Text elements used in other `.sketch` files are using a shared text style derived from here. This file contains an artboard for each text color. The respective color symbol is nested on top of each artboard for sampling and applying it for each text instance.

---

### Components

`libs/library-components.sketch`

| Constructors |
|:--- |
| <img src="img/constructors-dark.jpg" width="181" height="78"/> |

Constructors are elements that often serve no purpose in isolation but are repeatedly used within components and pre-compositions. Constructors are meant to control backgrounds, shapes, shadows etc.

| Components |
|:--- |
| <img src="img/components-dark.jpg" width="419" height="154"/> |

Components are design elements that are meaningful in isolation. For example buttons, text fields, radios and checkboxes fall under this category.

| Pre-compositions |
|:--- |
| <img src="img/pre-compositions-dark.jpg" width="720" height="249"/> |

Pre-compositions are collections of constructors and components that form more complex elements that are used repeatedly in compositions.

---

### Composition

`/composition.sketch`

<img src="img/composition.gif" width="660" height="470"/>

Composition presents fully designed static views of how the final product is expected to look.

---

## Workflows

When designing new views and features, it is better not to constrain yourself to working only with elements that are currently available in your design system. Sketch freely and update your libraries accordingly when reaching clarity on the wanted design solution. All of the library files are meant to be living documents that contain only elements that are actively used in compositions. 

## Setup
Clone this repository or download as a zip.

## Status

In development.
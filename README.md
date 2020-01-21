# OpenPeriodic
Open-sourced machine-readable periodic table data.

## Specification
In its simplest form, OpenPeriodic is a compiliation of YAML files representing all of the elements of the periodic table. On each release, the YAML files will be compiled into one single YAML file containing all of the elements.

### Element Files

| Key | Type | Description |
| --- | ---- | ----------- |
| **Basics** |
| `symbol` | String | The chemical symbol for the element. (e.g. H, He, Ar) |
| `name` | String | The chemical name. (e.g. Hydrogen, Helium, Argon) |
| `number` | Integer | The atomic number of the element. |
| `weight` | Float | The average atomic mass (or atomic weight) of the element. |
| **Classification** |
| `group` | Integer | The group (column) that the element is in. Leave out for lanthanoids and actinoids. |
| `period` | Integer | The period that the element is in. Also the number of energy levels at ground state. |
| `family` | [Family](#family) | The family that the element is part of. |

### Enumerations

#### Family
The family of the element. The acceptable values are listed below.
| Value | Description |
| ----- | ----------- |
| `alkali` | Alkali Metals (i.e. Metals in group 1) |
| `alkalineEarth` | Alkaline Earth Metals (i.e. Metals in group 2) |
| `transition` | Metals in the d-block, excluding group 12. |
| `postTransition` | Metals in the p-block, plus group 12. |
| `lanthanoid` | Lanthanoids (elements 57-71) |
| `actinoid` | Actinoids (elements 89-103) |
| `metalloid` | Metalloids |
| `reactive` | Reactive Nonmetals |
| `halogen` | Halogens (group 17) |
| `nobleGas` | Noble Gases (group 18) |
| `unknown` | Unclassified Elements |

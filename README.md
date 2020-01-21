# OpenPeriodic
Open-sourced machine-readable periodic table data.

## Specification
In its simplest form, OpenPeriodic is a compiliation of YAML files representing all of the elements of the periodic table. On each release, the YAML files will be compiled into one single YAML file containing all of the elements.

### Element Files

| Key | Type | Description |
| --- | ---- | ----------- |
| `symbol` | String | The chemical symbol for the element. (e.g. H, He, Ar) |
| `name` | String | The chemical name. (e.g. Hydrogen, Helium, Argon) |
| `number` | Integer | The atomic number of the element. |

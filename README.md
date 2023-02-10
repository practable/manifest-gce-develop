# manifest-gce-develop
Manifest for the gce-develop system (dev.practable.io)

## Naming scheme

### Type codes

The manifest type codes are one or two letter codes that distinguish between different types of entity. This convention emerged out of the short names used during testing, but seem likely to offer additional visual guidance to the eye on what section you are editing (you only need to scroll far enough to see a name to be sure what section of the manifest you are in):


| code | type        |
|------|-------------|
| g    | group       |
| p    | policy      |
| r    | resource    |
| sl   | slot        |
| st   | stream      |
| ui   | user interface |
| us   | user interface set |
| w    | window |


### Descriptions

All descriptions are done by reference, to reduce the size of the manifest when descriptions are repeated.

The format for the name of descriptions is as short as possible:

```
description format: d-<type>-<part1>[-<part2>[-<part3>]]
```
For example, the everyone group description is named `d-g-everyone`

Within the description, all fields may be displayed to users so should contain "normal language," i.e. name fields within descriptions should NOT contain type codes.

#### name

The title on any cards displayed to the user

#### short 

A self-contained single sentence description of the entity. Include any distinguishing parameters that sizxe of weight on a spinner, for example, because long descriptions may not be displayed.

#### long

A longer description that could be 2-3 sentences. Optional, may not be displayed anyway.

#### further 

A link to a webpage with further information. Optional, may not be shown anyway.

#### thumb

link to a 150x150 pixel png for display in small cards. Optional but recommended.Optional but recommended to help users find the right experiments in a screen with many options.

### image

link to a 500x500 pixel png for display in large cards. Optional but recommended for pleasing presentation to users.


### Names

To maintain consistency, each resource should be named in the manifest (i.e. the names start each entity in the YAML and NOT the name IN the description objects) as follows

```
name format: <type>-<part1>[-<part2>[-<part3>]]
```

For example, the everyone group is named `g-everyone`

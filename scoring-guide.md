# Scoring Guide

The Material Coverage project's mission is to assess the quality of design libraries
in an accurate and fair manner. To do this, design libraries are compared with
the [visual component specifications](https://material.io/components) provided
by Material Design.

## Status Levels
A library is graded on its ability to create each Material Design component using three distinct levels:

#### Nonexistant
This status is used when a library provides no guidance or is unable to make
a certain component. To surpass this level, a library must be able to create the
component in a rational way with some sort of guidance.

#### Partial
This status is used when a library can only partially make a certain component.
The partial status might be used if a library has a hard time replicating a
a core feature of a component. In addition, the partial
status may be used if a component is complete but somehow inconvenient for developers.

#### Complete
This status is used when a library can make a certain component's basic
behaviors. Extra-complicated and minor details are not assessed but core functionality
is. When this status is used, it is expected that specific guidance is given and a
simple version of the component can be created easily.

## Availability and Completeness Scoring
To assess a library's overall ability to recreate Material Components, we use a point
system to define a "score" for each Material component and divide by the whole. Based on
each certain status, a library is granted either 0, 0.5 or 1 point(s):


### Status Legened
| Status | Emoji Icon | Points Toward Availability Score | Points Toward Completeness Score |
| :---   | :---:      |:--:                              | :--:                             |
| Nonexistant| ❌ | 0 | 0 |
|Partial   | 🟡 |  1 | 0.5 |
|Complete   | ✅ | 1  | 1  |

Afterward, the total scores are divided by the amount of Material components available
(usually 26+) to generate a percentage. We do this twice to generate availability and completeness scores:

#### Availability (more commonly used)
This score assess how many components are able to be recreated in some fashion.
Since partial scores can sometimes be controversial, the availability score ignores
them and rounds the scores up to 1. This gives the public a better look into the
amount of components covered and how well a library can fit into a design system.

#### Completeness (less commonly used)
This score assess the developer experience of using a design library. Since partial
scores are considered 0.5, it gives developers a look into how janky or hacky
a certain library is. For example, if the library relies on a lot of system tooling for
its UI, then that will be reflected in a decrease of the completeness score.

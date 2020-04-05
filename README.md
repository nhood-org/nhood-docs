# nhood

## Problem

`nhood` (for neighborhood) is a data search engine based on a shortest geometrical distances between multidimensional metadata vectors. Engine maintains an universe of data with n-dimensional vectors of metadata as data description. On search the geometrically nearest objects are resolved and returned. 

## Use-cases

1. A resolution of nearest geographical locations around the user.
1. A resolution of content relevant to user preferences.

## Use-case examples

There is a couple of examples implemented on an engine library level as ready-to-run unit tests. You can find those in `nhood-engine/nhood-engine-examples` module.

Currently, the following use-cases are covered:

- DataFinder is used to resolve 30 of cities closest to Cracow considering its geographical coordinates.
- DataFinder is used to resolve a planet with the characteristics similar to the characteristics of the Earth.
- DataFinder is used to resolve 10 of songs similar to the given one according to its metadata vectors.

## Goal

The engine implementation if focused on:

- high performance
- resilience
- reactiveness
- cloud-nativeness

## Contribution

Would you like to contribute to `nhood` project? Feel free to have a look [here](./CONTRIBUTING.md).

## Road map

Road map may be found [here](./ROADMAP.md).

## License

All nhood components and documentation is released under the MIT license:
- https://opensource.org/licenses/MIT

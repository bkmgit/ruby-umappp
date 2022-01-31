# Umap

🗺️ [Umappp](https://github.com/LTLA/umappp) - Uniform Manifold Approximation and Projection - for Ruby

* Compatible with [yaumap](https://github.com/LTLA/yaumap/blob/master/R/umap_from_matrix.R)
* Support [Numo::NArray](https://github.com/ruby-numo/numo-narray)

🚧 alpha - Still in development.

## Installation

```
git clone https://github.com/kojix2/umap
cd umap
rake compile
rake install
```

* OpenMP is required for multithreading.

## Usage

```ruby
Umap.umap(pixels, nthreads: 4)
```

Parameters and default values

```markdown
- method               : :annoy (another option is vptree)
- ndim                 : 2
- nthreads             : 2 (OpenMP required)
- tick                 : 0 (Not yet implemented)

<umappp parameters>

- local_connectivity   : 1.0
- bandwidth            : 1
- mix_ratio            : 1
- spread               : 1
- min_dist             : 0.01
- a                    : 0
- b                    : 0
- repulsion_strength   : 1
- num_epochs           : 500
- learning_rate        : 1
- negative_sample_rate : 5
- num_neighbors        : 15
- seed                 : 1234567890
- batch                : false
```

## Development

* [numo.hpp](https://github.com/ankane/numo.hpp)
* [rice](https://github.com/jasonroelofs/rice)

## Contributing

Welcome!

## License

* As for the code I wrote, it is MIT.
* For other codes, please check on your own.

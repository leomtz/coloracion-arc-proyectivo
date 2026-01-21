## Authors

**Leonardo Martínez-Sandoval** ([Google Scholar](https://scholar.google.es/citations?hl=es&pli=1&user=hUjL-FwAAAAJ))  
**Gabriela Araujo-Pardo** ([Google Scholar](https://scholar.google.es/citations?user=btyNjrYAAAAJ&hl=es))


# Coloring the Euclidean Grid and Affine Planes

This repository accompanies a research paper on exact colorings of finite grids, focusing on the Euclidean grid $[n]^2$ and the affine plane $AG(2,q)$. The included Jupyter notebooks implement efficient algorithms to find colorings that avoid monochromatic collinear triples, and explore the structure of maximal arcs and their colorings.

## Notebooks

### clean_euclidean.ipynb
Implements a backtracking coloring solver for the Euclidean grid $[n]^2$ using the Minimum Remaining Values (MRV) heuristic and forward checking. The notebook:

- Defines the grid and collinearity test (integer determinant).
- Searches for the minimal number of colors needed to avoid monochromatic collinear triples for $n=1$ to $n=9$.
- Explores the construction of maximal general position sets (arcs) with recursive algorithms.
- Finds collections of pairwise disjoint maximal arcs.
- Visualizes colorings and arcs using matplotlib.
- Saves results to text files in the `results_euclidean/` directory.


### clean_projective.ipynb
Studies colorings for the affine plane $AG(2,q)$, with supporting code for the projective plane $PG(2,q)$. It implements:

- Construction of the affine and projective planes, and collinearity relations.
- Exact coloring algorithms for $AG(2,q)$.
- Search for minimal colorings and maximal arcs in the affine setting.
- Visualization and result export.

## Dependencies

The code is designed to be minimal and portable. The only non-standard dependency is:

- `matplotlib` (for visualization)

All other code uses only the Python standard library and common scientific packages (e.g., `itertools`, `functools`, `typing`).

## Example Output

Below is a sample visualization of a coloring (see `output.png`):

![Sample coloring output](output.png)

## How to Cite

If you use this code or results in your work, please cite the accompanying paper. A BibTeX entry will be provided here:


```bibtex
@article{martinez2026arcchromatic,
	title={The arc chromatic number for Galois projective planes, affine planes and Euclidean grids},
	author={Araujo-Pardo, Gabriela and Martínez-Sandoval, Leonardo},
	journal={arXiv preprint},
	year={2026},
	eprint={TBD},
	url={TBD}
}
```

---
For questions or suggestions, please open an issue or contact the authors.

# Changelog

All notable changes to this project will be documented in this file.

## [1.4.1] - 2020/11/29

### Added

- New ``solve_ls`` function to solve linear Least Squares problems

### Fixed

- Call to ``print`` in PyPI description
- Handling of quadprog ValueError exceptions

## [1.4] - 2020/07/04

### Added

- Solver settings can now by passed to ``solve_qp`` as keyword arguments
- Started an [API documentation](https://scaron.info/doc/qpsolvers/)

### Changed

- Made ``verbose`` an explicit keyword argument of all internal functions
- OSQP settings now match precision of other solvers (thanks to @Neotriple)

## [1.3.1] - 2020/06/13

### Fixed

- Equation of quadratic program on [PyPI page](https://pypi.org/project/qpsolvers/)

## [1.3] - 2020/05/16

### Added

- Lower and upper bound keyword arguments ``lb`` and ``ub``

### Fixed

- Check that equality/inequality matrices/vectors are provided consistently
- Relaxed offset check in [test\_solvers.py](examples/test_solvers.py)

## [1.2.1] - 2020/05/16

### Added

- cvxpy: verbose keyword argument
- ecos: verbose keyword argument
- gurobi: verbose keyword argument
- osqp: verbose keyword argument

### Fixed

- Ignore verbosity argument when solver is not available

## [1.2] - 2020/05/16

### Added

- cvxopt: verbose keyword argument
- mosek: verbose keyword argument
- qpoases: verbose keyword argument

## [1.1.2] - 2020/05/15

### Fixed

- osqp: handle both old and more recent versions

## [1.1.1] - 2020/05/15

### Fixed

- Avoid variable name clash in OSQP
- Handle quadprog exception to avoid confusion on cost matrix notation

## [1.1] - 2020/03/07

### Added

- ECOS solver interface (no need to go through CVXPY any more)
- Update ECOS performance in benchmark (much better than before!)

### Fixed

- Fix link to ECOS in setup.py
- Remove ned for IPython in solver test
- Update notes on P matrix

## [1.0.7] - 2019/10/26

### Changed

- Always reshape A or G vectors into one-line matrices

### Fixed

- cvxopt: handle case where G and h are None but not A and b
- osqp: handle case where G and h are None
- osqp: handle case where both G and A are one-line matrices
- qpoases: handle case where G and h are None but not A and b

## [1.0.6] - 2019/10/26

Thanks to Brian Delhaisse and Soeren Wolfers who contributed fixes to this
release!

### Fixed

- quadprog: handle case where G and h are None
- quadprog: handle cas where A.ndim == 1
- Make examples compatible with both Python 2 and Python 3

## [1.0.5] - 2019/04/10

### Added

- Equality constraint shown in the README example
- Installation file ``requirements.txt``
- Installation instructions for qpOASES
- OSQP: automatic CSC matrix conversions (with performance warnings)
- This change log

### Fixed

- CVXOPT: case where A is one-dimensional
- qpOASES: case where both G and A are not None
- quadprog: wrapper for one-dimensional A matrix (thanks to @nvitucci)

### Changed

- CVXOPT version is now 1.1.8 due to [this issue](https://github.com/urinieto/msaf-gpl/issues/2)
- Examples now in a [separate folder](examples)

## [1.0.4] - 2018/07/05

### Added
- Let's take this change log from there.

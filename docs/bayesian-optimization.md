# bayesian-optimization

Bayesian optimization (BO) is a black-box global optimization algorithm. During the process, this algorithm determines the next sampling point based on Bayesian inference of the latent function.

BO is likely to find reasonable solutions with fewer function evaluations than other optimization algorithms. Thus, it is suitable for problems with expensive-to-evaluate objective functions.

## Header

```cpp
#include <mathtoolbox/bayesian-optimization.hpp>
```

## Internal Dependencies

- [acquisition-functions](../acquisition-functions)
- [gradient-descent](../gradient-descent)
- [gaussian-process-regression](../gaussian-process-regression/)

## Math and Algorithm

(TODO)

## Examples

The following plot shows a result of optimizing a simple objective function:
$$
\max_{\mathbf{x} \in [-1, 1]^{5}} \{ - \| \mathbf{x} \|^{2} \}
$$
50 times with random initial solutions. As a baseline, it also shows a result by the same setting except for using random uniform sampling instead of BO.

![](./bayesian-optimization/bo-vs-rand.png)

## Useful Resources

- Yuki Koyama, Issei Sato, Daisuke Sakamoto, and Takeo Igarashi. 2017. Sequential line search for efficient visual design optimization by crowds. ACM Trans. Graph. 36, 4, pp.48:1--48:11 (2017). DOI: <https://doi.org/10.1145/3072959.3073598>
- (TODO)
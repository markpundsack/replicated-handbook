# Product Principles

These are some product principles that came out of a Product Offsite \(July 2021\). Some of these are more aspirational than actual, but should drive future development work.

1. Composable features/products \(on and off ramps\)
   1. Components should be optional \(ex: admin console GUI, license management\).
   2. End users should be able to use infrastructure as code without the GUI. Batteries included but swappable \(ex: vendor connects their license system\).
2. Streamlined user experience flows
   1. Even if features are composable, we also need to make streamlined flows to solve user jobs by composing those features into a great overall flow.
   2. Delightful experiences are how we win \(ease of use/time to success\).
3. Observability/debuggability/troubleshooting
   1. Don’t just design for the golden path, make a great experience when things go wrong. Make sure people know what has happened, what went wrong, ideally how to fix it, and if they do fix it, make it easy to start where it left off. Support and maintainability.
4. CLI-first
   1. Emphasize CLI-first during implementation, CLI shouldn’t be an afterthought.

Also see [Engineering Principles](https://wiki.replicated.io/doc/engineering-principals-kGYvQmwdJC).


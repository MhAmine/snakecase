# snakecase 0.2.2

* introduced `to_any_case()` (all functionality and documentation provided, but implementation has to be cleaned and also tests have to be written)

# snakecase 0.2.1

* fixed bug: `to_snake_case_dev(c("ssRRss"))` returns now `ss_r_rss` instead of`"ss_r_r_ss"`
* `to_snake_case()` now treats only spaces like underscores now (not dots anymore)
* functionality to treat different stuff like dots will be added via a new function:  
`to_any_case()`, which will wrap the other three and will have pre- and postprocess arguments

# snakecase 0.2.0

* renamed the single input parameters consistent to `string` (without deprecating
the old name before, since the package was in early dev-stage anyway).
* started a to develop and implement consistent logic (which still has to be better documented in the readme)
* introduced tests for more hard coded examples and the logic behind it (still more
hardcoded examples and a third part of the logic have to be tested)
* internal logic has been simplified and modularised a lot, which makes it easier
to maintain and introduce more highlevel features in the future
* added integrated tests via appveyor on windows
* added badges for cran status and codecoverage to readme

# snakecase 0.1.0

* Introduced `to_snake_case()` which converts strings to snake_case.
* added functions `to_small_camel_case()` and `to_big_camel_case()` which internally
build up on `to_snake_case()` and convert to the appropriate target case.
* added basic hard coded tests
* added integrated tests on linux via travis.ci



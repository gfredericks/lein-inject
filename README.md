# Hi Colin!

To try this out, run `lein install` and then add the following to the
`project.clj` of some project, and make sure it's not using clojure 1.9:

``` clojure
:plugins [[com.palletops/lein-shorthand "0.4.1-SNAPSHOT"]]
:shorthand {. [clojure.test/run-tests]}
```

Then after starting a repl, `./run-tests` should resolve to a function.

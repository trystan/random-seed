# random-seed

Supply your own random seed to the clojure.core random functions.

## Leiningen

    [random-seed "1.0.0"]

## Usage

    (ns example.core
      (:require [random-seed.core :refer :all])
      (:refer-clojure :exclude [rand rand-int rand-nth shuffle]))

    (set-random-seed! 888)

    (rand 5)

    (rand-int 30)

    (rand-nth [:a :b :c])

    (shuffle [:a :b :c])

## License

Copyright © 2015 Trystan

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.

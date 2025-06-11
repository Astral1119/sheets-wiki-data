The [CORE library](https://docs.google.com/spreadsheets/d/13UCmWS5fzYTqxzRI5iEaJnc9ad9poMm6ZyxX9HlYbGE) provides implementations for functional data structures and a suite of helper functions for mid-level manipulation.

Currently, the only data structure implemented is `CHVEC`.

### General principles

Containers in the CORE library all have an abstracted interface. They can be interacted with via payloads.

Payloads can be methods or values. To 

### CHVEC

`CHVEC` (from [[CHoose]] VECtor) is a Clojure-style vector implemented using array mapped [tries](https://en.wikipedia.org/wiki/Trie). It supports efficient random access.
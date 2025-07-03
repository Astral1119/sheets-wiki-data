---
version: 0.1.1
maintainer: Astral Café
last-updated: 2025-06-12
title: anduin
tags:
  - anduin
---

Anduin (/ˈanduɪn/) brings advanced [functional](https://en.wikipedia.org/wiki/Functional_programming) and [object-oriented](https://en.wikipedia.org/wiki/Object-oriented_programming) programming concepts to Google Sheets.

### Code sample

```gse
=let(
  pet_record, record("pet")({"name", "species", "age", "weight"}),

  customer_protocol, protocol({"add_pet", "get_pet"}),

  customer_record, record("customer")

    ({"name", "address", "phone", "email", "pets"})

    (customer_protocol)

    ("add_pet")
    (lambda(self, lambda(pet,
        self(method("update"))("pets", self("pets")(method("update"))(pet("name"), pet))
    )))

    ("get_pet")
    (lambda(self, lambda(petname,
      self("pets")(petname)
    ))),

  customer_instance, customer_record
    ("John Doe")
    ("123 Main St")
    ("555-1234")
    ("johndoe@example.com")
    (DICT),
  
  fluffy, pet_record("Fluffy")("cat")(3)(10),
  cpt_arf, pet_record("Cpt. Arf")("dog")(5)(20),
  updated_customer, customer_instance(method("add_pet"))(fluffy),
  fluffy_retrieved, updated_customer(method("get_pet"))("Fluffy"),
  fluffy_retrieved("name")&" is a "&fluffy_retrieved("species")&" and is "&fluffy_retrieved("age")&" years old."
)
```

`Fluffy is a cat and is 3 years old.`
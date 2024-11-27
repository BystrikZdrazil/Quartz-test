---
title: "Oracle"
draft: false
tags:
  - 
---
In [[Software testing]], a **test oracle** (or just **oracle**) is a provider of information that describes [correct](https://en.wikipedia.org/wiki/Correctness_(computer_science) "Correctness (computer science)") output based on the input of a [test case](https://en.wikipedia.org/wiki/Test_case "Test case"). Testing with an oracle involves comparing actual results of the system under test (SUT) with the expected results as provided by the oracle.[[1]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-1)

The term "test oracle" was first introduced in a paper by William E. Howden.[[2]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-2) Additional work on different kinds of oracles was explored by [Elaine Weyuker](https://en.wikipedia.org/wiki/Elaine_Weyuker "Elaine Weyuker").[[3]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-3)

An oracle can operate separately from the SUT; accessed at test [runtime](https://en.wikipedia.org/wiki/Runtime_(program_lifecycle_phase) "Runtime (program lifecycle phase)"), or it can be used before a test is run with expected results encoded into the test logic.[[4]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-038720881X-4)

However, [method](https://en.wikipedia.org/wiki/Method_(computer_programming) "Method (computer programming)") postconditions are part of the SUT, as automated oracles in [design by contract](https://en.wikipedia.org/wiki/Design_by_contract "Design by contract") models.[[5]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-5)

Determining the correct output for a given input (and a set of program or system states) is known as the _oracle problem_ or _test oracle problem_,[[6]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-Oracle_survey-6): 507  which some consider a relatively hard problem, and involves working with problems related to controllability and observability.[[7]](https://en.wikipedia.org/wiki/Test_oracle#cite_note-ammann-intro-7)
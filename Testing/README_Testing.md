# Testing

## Testing Pyramid

- The testing pyramid is a visualization of how much testing should be done on which level. It looks like the following:

```java

                                   /\
                                  /  \
                                 /    \
                                /      \
                               /        \
                              /          \
                             /            \
                            /              \
                           /                \
                          /                  \
                         /                    \
                        /                      \
                       /                        \
                      /                          \
                     /............................\
                    / | Exploratory/Manual Testing|\
                   /  ............................. \
                  /           MANUAL TEST            \
                 /------------------------------------\
                /       ...............................\
               /        | E2E Testing/System testing  | \                    CI triggered
              /         ...............................  \
             /                  UI TESTS                  \ 
            /           Testing through a user interface   \
           /------------------------------------------------\
          /     ........................................     \
         /      |Build Acceptance/Regression Testing   |      \              CI triggered
        /       .......................................        \
       /                   INTEGRATION TESTS                     \
      /     Testing across integration of more than one system    \
     /-----------------------------------------------------        \
    /                    .............................              \
   /                     | Per code commit/Post Commit|              \
  /                      ..............................               \       Dev triggered
 /                               UNIT TESTING                          \      
/                        Testing isolated units of code                 \
-------------------------------------------------------------------------\

```

- The lower part of the test is more automated, which makes these tests faster.
- The more upward we go in the pyramid, the number of tests decreases.
- Please read [The Practical Test Pyramid](https://martinfowler.com/articles/practical-test-pyramid.html) by **Martin Fowler** for much, much more detailed information as he explains it better than I do.
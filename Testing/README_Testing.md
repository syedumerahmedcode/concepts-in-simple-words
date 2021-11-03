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
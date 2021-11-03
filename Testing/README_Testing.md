# Testing

## Testing Pyramid

- The testing pyramid is a visualization of how much testing should be done on which level. It looks like the following:

```xml



         /
        /				........................................
       /						INTEGRATION TESTS
      /                 Testing across integration of more than one system
     /-----------------------------------------------------
    /			     ..............................
   /					| Per code commit/Post Commit|
  /					..............................
 /							UNIT TESTING
/					Testing isolated units of code
--------------------------------------------------------------------------------------------------------------------------------

```
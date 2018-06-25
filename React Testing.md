# React Testing

## Test levels
- Unit -> Integration -> E2E
- Fast ---------------> Slow
- Cheap ---------> Expensive
- Less -----> More Confident
- Focus on integration
  - Balance the three parameters
  - Good integration test -> no need for unit test

## Bad Test
- Implementation Details
  - Test something API/Interface not provided
  - Refactor breaking test

## Good Test
- User Perspective
  - Test "what" user sees
  - Imitate "how" user uses

## Tools
- Enzyme vs. ReactDOM
  - Aware that some tools may not be required for essential functionalities

## react-testing-library
> arrange - act - assert
- render
  - get element DOM-wise
- simulate
- etc.

## E2E - Cypress (cypress-testing-library)
- All-in-one
- Time trael
- Screenshots / Videos
- etc.
# React Design Patterns

## Software Quality Triad
- Good - Fast - Cheap
- Can choose only two from three

## Dumb Components
- More components prone to duplicate handler
- Lots of dumb components tends to have that problem

## Higher-order Component
- Wrapper of dumb component with enhanced logics
- Give dumb components configurability
- Reusable & composable
- convention:
```js
enhance(options)(component)
enhance(component, options)
```
- Downsides:
  - No direct refernce to props provider
  - Leaky abstraction
  - Props collision
  - Harms readability when misused
  - Pollutes component tree
  - Polluted with wrappers

## Render Props (Function as a Children)
- Parent provides data, children decides how to render
- Make it clear how data is provided and consumed
```js
render() {
  const { data, loading, error } = this.state
  return this.props.children(data, loading, error)
}
```

## Utility Functions
- Abstraction repeated & lengthy functions

## Code Splitting
- Convert from type to features
```
src/
  reduces/
    component1.js
    component2.js
  components/
    1.js
    2.js
  actions/
```
```
src/
  feature-1/
    reducer.js
    component.js
    action.js
  feature-2/
```
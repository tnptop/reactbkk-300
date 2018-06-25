# Opening Keynote

## React async Rendering
- adapt to user's device and network
- fast interactions feel instant
- slow interactions feel responsive

## Deprecation of React Lifecycles
- Encourage misuse -> unexpected bug
- Especially when async rendering
- New lifecycle to support same use cases
### Deprecated
- componentWillMount()
- componentWillUpdate()
- componentWillReceiveProps()

## React Native Re-architecture
- New thread model to handle high-priority updates better
- Async rendering
- Faster bridge and lighter weight
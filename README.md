# jecs-topo-runtime

This package does not really depend on the jecs functionality.
I'm not sure whether this package will eventually be branched out into an abstract topo runtime package.

## Setup

```ts
const world = new World()
const loop = new Loop(world, ...whatever other arguments)

const connections = loop.begin({
    default: RunService.Heartbeat,
})

const system = () => {}

loop.scheduleSystem(system)

// hot reload stuff
loop.evictSystem(system)
```

## Builtin hooks

useEvent
useThrottle

There is `useHookState` function for implementing custom hooks.

## Side note

Not a single test has been written for the package so it may contain
There has not been written any test

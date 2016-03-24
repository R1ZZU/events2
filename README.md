# events2

ES2015 implementation of nodejs EventEmitter

## Descrirption

This node module is a clone of nodejs [EventEmitter](https://https://nodejs.org/dist/latest-v5.x/docs/api/events.html)

## Why?

ES2015 is awesome, so why not?

 * highly readable
 * `class` instead of constructor `function EventEmitter`
 * `Map()` instead of `{}` as events storage
 * `Set()` instead of array as event listener storage
 * `Array.from(arguments)` instead of `[].slice.call`

## What's different from core EventEmitter?

 * `emitter.off([eventName, listener])` method

   This is an alias for core `emitter.removeListener` AND `emitter.removeAllListeners`. Removes all listeners, or those of the specified event, or specified listener.
 * no `defaultMaxListeners` limit
 * as a result – no `listenerCount()` and `getMaxListners()`
 * no `listeners()` and `listenersCount()`
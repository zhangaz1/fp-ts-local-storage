[fp-ts](https://github.com/gcanti/fp-ts) bindings for LocalStorage

# Documentation

- [API Reference](https://gcanti.github.io/fp-ts-local-storage)

# Example

```ts
import { setItem, getItem } from 'fp-ts-local-storage'

const program = setItem('foo', JSON.stringify({ bar: 'baz' })).chain(() => getItem('foo'))

console.log(program.run()) // => some('{"bar":"baz"}')
```

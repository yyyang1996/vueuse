---
category: Sensors
---

# useOnline

Reactive online state. A wrapper of `useNetwork`.

## Usage

```js
import { useOnline } from '@vueuse/core'

const online = useOnline()
```


<!--FOOTER_STARTS-->
## Type Declarations

```typescript
/**
 * Reactive online state.
 *
 * @link https://vueuse.org/useOnline
 * @param options
 */
export declare function useOnline(options?: ConfigurableWindow): Ref<boolean>
```

## Source

[Source](https://github.com/vueuse/vueuse/blob/main/packages/core/useOnline/index.ts) • [Demo](https://github.com/vueuse/vueuse/blob/main/packages/core/useOnline/demo.vue) • [Docs](https://github.com/vueuse/vueuse/blob/main/packages/core/useOnline/index.md)


<!--FOOTER_ENDS-->

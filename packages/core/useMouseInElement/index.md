---
category: Sensors
---

# useMouseInElement

Reactive mouse position related to an element

## Usage

```html {15}
<template>
  <div ref="target">
    <h1>Hello world</h1>
  </div>
</template>

<script>
import { ref } from 'vue'
import { useMouseInElement } from '@vueuse/core'

export default {
  setup() {
    const el = ref(null)

    const { x, y, isOutside } = useMouseInElement(el)

    return { x, y, isOutside }
  }
}
</script>
```


<!--FOOTER_STARTS-->
## Type Declarations

```typescript
export interface MouseInElementOptions extends MouseOptions {
  handleOutside?: boolean
}
/**
 * Reactive mouse position related to an element.
 *
 * @link https://vueuse.org/useMouseInElement
 * @param target
 * @param options
 */
export declare function useMouseInElement(
  target?: MaybeElementRef,
  options?: MouseInElementOptions
): {
  x: Ref<number>
  y: Ref<number>
  sourceType: Ref<MouseSourceType>
  elementX: Ref<number>
  elementY: Ref<number>
  elementPositionX: Ref<number>
  elementPositionY: Ref<number>
  elementHeight: Ref<number>
  elementWidth: Ref<number>
  isOutside: Ref<boolean>
  stop: () => void
}
```

## Source

[Source](https://github.com/vueuse/vueuse/blob/main/packages/core/useMouseInElement/index.ts) • [Demo](https://github.com/vueuse/vueuse/blob/main/packages/core/useMouseInElement/demo.vue) • [Docs](https://github.com/vueuse/vueuse/blob/main/packages/core/useMouseInElement/index.md)


<!--FOOTER_ENDS-->

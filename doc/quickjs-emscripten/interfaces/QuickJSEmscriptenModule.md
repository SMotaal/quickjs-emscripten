[quickjs-emscripten](../../packages.md) • **quickjs-emscripten** • [Readme](../README.md) \| [Exports](../exports.md)

***

[quickjs-emscripten](../../packages.md) / [quickjs-emscripten](../exports.md) / QuickJSEmscriptenModule

# Interface: QuickJSEmscriptenModule

Typings for the features we use to interface with our Emscripten build of
QuickJS.

## Contents

- [Extends](QuickJSEmscriptenModule.md#extends)
- [Properties](QuickJSEmscriptenModule.md#properties)
  - [FAST\_MEMORY](QuickJSEmscriptenModule.md#fast-memory)
  - [HEAP16](QuickJSEmscriptenModule.md#heap16)
  - [HEAP32](QuickJSEmscriptenModule.md#heap32)
  - [HEAP8](QuickJSEmscriptenModule.md#heap8)
  - [HEAPF32](QuickJSEmscriptenModule.md#heapf32)
  - [HEAPF64](QuickJSEmscriptenModule.md#heapf64)
  - [HEAPU16](QuickJSEmscriptenModule.md#heapu16)
  - [HEAPU32](QuickJSEmscriptenModule.md#heapu32)
  - [HEAPU8](QuickJSEmscriptenModule.md#heapu8)
  - [TOTAL\_MEMORY](QuickJSEmscriptenModule.md#total-memory)
  - [TOTAL\_STACK](QuickJSEmscriptenModule.md#total-stack)
  - [callbacks](QuickJSEmscriptenModule.md#callbacks)
  - [type](QuickJSEmscriptenModule.md#type)
- [Methods](QuickJSEmscriptenModule.md#methods)
  - [UTF8ToString()](QuickJSEmscriptenModule.md#utf8tostring)
  - [\_free()](QuickJSEmscriptenModule.md#free)
  - [\_malloc()](QuickJSEmscriptenModule.md#malloc)
  - [cwrap()](QuickJSEmscriptenModule.md#cwrap)
  - [lengthBytesUTF8()](QuickJSEmscriptenModule.md#lengthbytesutf8)
  - [stringToUTF8()](QuickJSEmscriptenModule.md#stringtoutf8)

## Extends

- [`EmscriptenModule`](EmscriptenModule.md)

## Properties

### FAST\_MEMORY

> **FAST\_MEMORY**: `number`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.FAST_MEMORY`](EmscriptenModule.md#fast-memory)

#### Source

quickjs-ffi-types/dist/index.d.ts:165

***

### HEAP16

> **HEAP16**: `Int16Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAP16`](EmscriptenModule.md#heap16)

#### Source

quickjs-ffi-types/dist/index.d.ts:156

***

### HEAP32

> **HEAP32**: `Int32Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAP32`](EmscriptenModule.md#heap32)

#### Source

quickjs-ffi-types/dist/index.d.ts:157

***

### HEAP8

> **HEAP8**: `Int8Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAP8`](EmscriptenModule.md#heap8)

#### Source

quickjs-ffi-types/dist/index.d.ts:155

***

### HEAPF32

> **HEAPF32**: `Float32Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAPF32`](EmscriptenModule.md#heapf32)

#### Source

quickjs-ffi-types/dist/index.d.ts:161

***

### HEAPF64

> **HEAPF64**: `Float64Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAPF64`](EmscriptenModule.md#heapf64)

#### Source

quickjs-ffi-types/dist/index.d.ts:162

***

### HEAPU16

> **HEAPU16**: `Uint16Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAPU16`](EmscriptenModule.md#heapu16)

#### Source

quickjs-ffi-types/dist/index.d.ts:159

***

### HEAPU32

> **HEAPU32**: `Uint32Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAPU32`](EmscriptenModule.md#heapu32)

#### Source

quickjs-ffi-types/dist/index.d.ts:160

***

### HEAPU8

> **HEAPU8**: `Uint8Array`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.HEAPU8`](EmscriptenModule.md#heapu8)

#### Source

quickjs-ffi-types/dist/index.d.ts:158

***

### TOTAL\_MEMORY

> **TOTAL\_MEMORY**: `number`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.TOTAL_MEMORY`](EmscriptenModule.md#total-memory)

#### Source

quickjs-ffi-types/dist/index.d.ts:164

***

### TOTAL\_STACK

> **TOTAL\_STACK**: `number`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.TOTAL_STACK`](EmscriptenModule.md#total-stack)

#### Source

quickjs-ffi-types/dist/index.d.ts:163

***

### callbacks

> **callbacks**: `EmscriptenModuleCallbacks`

#### Source

quickjs-ffi-types/dist/index.d.ts:201

***

### type

> **type**: `"sync"`

#### Source

quickjs-ffi-types/dist/index.d.ts:200

## Methods

### UTF8ToString()

> **UTF8ToString**(`ptr`, `maxBytesToRead`?): `string`

HeapChar to JS string.
https://emscripten.org/docs/api_reference/preamble.js.html#UTF8ToString

#### Parameters

• **ptr**: [`BorrowedHeapCharPointer`](../exports.md#borrowedheapcharpointer)

• **maxBytesToRead?**: `number`

#### Returns

`string`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.UTF8ToString`](EmscriptenModule.md#utf8tostring)

#### Source

quickjs-ffi-types/dist/index.d.ts:150

***

### \_free()

> **\_free**(`ptr`): `void`

#### Parameters

• **ptr**: `number`

#### Returns

`void`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule._free`](EmscriptenModule.md#free)

#### Source

quickjs-ffi-types/dist/index.d.ts:153

***

### \_malloc()

> **\_malloc**(`size`): `number`

#### Parameters

• **size**: `number`

#### Returns

`number`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule._malloc`](EmscriptenModule.md#malloc)

#### Source

quickjs-ffi-types/dist/index.d.ts:152

***

### cwrap()

> **cwrap**(`ident`, `returnType`, `argTypes`, `opts`?): (...`args`) => `any`

#### Parameters

• **ident**: `string`

• **returnType**: `null` \| `ValueType`

• **argTypes**: `ValueType`[]

• **opts?**: `CCallOpts`

#### Returns

`Function`

> ##### Parameters
>
> • ...**args**: `any`[]
>
> ##### Returns
>
> `any`
>

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.cwrap`](EmscriptenModule.md#cwrap)

#### Source

quickjs-ffi-types/dist/index.d.ts:154

***

### lengthBytesUTF8()

> **lengthBytesUTF8**(`str`): `number`

#### Parameters

• **str**: `string`

#### Returns

`number`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.lengthBytesUTF8`](EmscriptenModule.md#lengthbytesutf8)

#### Source

quickjs-ffi-types/dist/index.d.ts:151

***

### stringToUTF8()

> **stringToUTF8**(`str`, `outPtr`, `maxBytesToRead`?): `void`

Write JS `str` to HeapChar pointer.
https://emscripten.org/docs/api_reference/preamble.js.html#stringToUTF8

#### Parameters

• **str**: `string`

• **outPtr**: [`OwnedHeapCharPointer`](../exports.md#ownedheapcharpointer)

• **maxBytesToRead?**: `number`

#### Returns

`void`

#### Inherited from

[`quickjs-emscripten.EmscriptenModule.stringToUTF8`](EmscriptenModule.md#stringtoutf8)

#### Source

quickjs-ffi-types/dist/index.d.ts:145

***

Generated using [typedoc-plugin-markdown](https://www.npmjs.com/package/typedoc-plugin-markdown) and [TypeDoc](https://typedoc.org/)
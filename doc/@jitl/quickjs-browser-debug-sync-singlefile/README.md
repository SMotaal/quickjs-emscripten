[quickjs-emscripten](../../packages.md) • **@jitl/quickjs-browser-debug-sync-singlefile** • [Readme](README.md) \| [Exports](exports.md)

***

# @jitl/quickjs-browser-debug-sync-singlefile

ESModule for browsers or browser-like environments

This generated package is part of [quickjs-emscripten](https://github.com/justjake/quickjs-emscripten).
It contains a variant of the quickjs WASM library, and can be used with quickjs-emscripten-core.

```typescript
import variant from "@jitl/quickjs-browser-debug-sync-singlefile"
import { newQuickJSWASMModuleFromVariant } from "quickjs-emscripten-core"
const QuickJS = await newQuickJSWASMModuleFromVariant(variant)
```

This variant was built with the following settings:

## Contents

- [Library: quickjs](README.md#library-quickjs)
- [Release mode: debug](README.md#release-mode-debug)
- [Module system: esm](README.md#module-system-esm)
- [Extra async magic? No](README.md#extra-async-magic-no)
- [Single-file, or separate .wasm file? singlefile](README.md#single-file-or-separate-wasm-file-singlefile)
- [More details](README.md#more-details)

## Library: quickjs

The original [bellard/quickjs](https://github.com/bellard/quickjs) library.

## Release mode: debug

Enables assertions and memory sanitizers. Try to run your tests against debug variants, in addition to your preferred production variant, to catch more bugs.

## Module system: esm

This variant exports an ESModule, which is standardized for browsers and more modern browser-like environments. It cannot be imported from CommonJS without shenanigans.

## Extra async magic? No

The default, normal build. Note that both variants support regular async functions.

## Single-file, or separate .wasm file? singlefile

The WASM runtime is included directly in the JS file. Use if you run into issues with missing .wasm files when building or deploying your app.

## More details

Full variant JSON description:

```json
{
  "library": "quickjs",
  "releaseMode": "debug",
  "syncMode": "sync",
  "emscriptenInclusion": "singlefile",
  "description": "ESModule for browsers or browser-like environments",
  "emscriptenEnvironment": ["web", "worker"],
  "moduleSystem": "esm"
}
```

Variant-specific Emscripten build flags:

```json
[
  "-O0",
  "-DQTS_DEBUG_MODE",
  "-gsource-map",
  "-s ASSERTIONS=1",
  "-s SINGLE_FILE=1",
  "-s EXPORT_ES6=1",
  "-s ENVIRONMENT=web,worker",
  "-DQTS_SANITIZE_LEAK",
  "-fsanitize=leak",
  "-g2",
  "-s ASYNCIFY_ADVISE=1",
  "-O3"
]
```

***

Generated using [typedoc-plugin-markdown](https://www.npmjs.com/package/typedoc-plugin-markdown) and [TypeDoc](https://typedoc.org/)
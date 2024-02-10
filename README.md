# Yeet
One day, JavaScript will have [`throw` expressions](https://github.com/tc39/proposal-throw-expressions). Until then, yeet!
```typescript
function save(filename = yeet("Argument required")) { ... }

const encoder = encoding === "utf8" ? new UTF8Encoder() 
              : encoding === "utf16le" ? new UTF16Encoder(false) 
              : encoding === "utf16be" ? new UTF16Encoder(true) 
              : yeet(TypeError, "Unsupported encoding");

class Product {
  get id() { return this._id; }
  set id(value) { this._id = value ?? yeet("Invalid value"); }
}
```

## Install
### NPM
```bash
npm install yeet-ts
# or
pnpm install yeet-ts
# or
bun install yeet-ts
```
... and then
```typescript
import { yeet } from "yeet-ts";
```

### Deno
```typescript
import { yeet } from "https://deno.land/x/yeet@v1.0.1/src/mod.ts";
```


## Contribute

To install dependencies:

```bash
bun install
```

To build:

```bash
bun run build
```

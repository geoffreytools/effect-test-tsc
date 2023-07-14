This repo is using `tsc` for building

`tsconfig.json/compilerOptions` includes `"declarations": true`.

I get the following error both in the workspace and during compilation:
> The inferred type of 'Foo' cannot be named without a reference to '../node_modules/@effect/data/Equal'. This is likely not portable. A type annotation is necessary.

no `.d.ts` file is emitted.

adding `"types": [ "@effect/data/Equal" ]` to `tsconfig.json` has no effect.
# TypeScript Complete Course - Beginner To Advanced + Project

## Introduction

### What include in the course?

- Module 1: All about types

  - Primitive types
  - Object types
  - Array types
  - Advance types
  - Type inference

- Module 2: Functions in TS

  - Declaring functions
  - Default and optional parameters
  - Custom parameters
  - Custom returns
  - Call signatures

- Module 3: Generics in TS

  - Polymorphic functions
  - Problems with function overloads
  - Intro to generics
  - Working with generics
  - Practice Implementations

- Module 4: Classes and Inheritance

  - Classes
  - Instances
  - Constructor functions
  - Inheritance
  - Access modifiers
  - Accessors and mutators

- Module 5: Abstract Classes and Interfaces

  - Static Properties
  - Abstract classes
  - Why abstract classes and differences
  - Interfaces
  - Multiple Inheritance
  - Generics with Interfaces

- Module 6: The TS Compiler

  - File options
  - Type checking options
  - File watcher and source maps

- Module 7: Prototypes and Objects

  - `this` keyword
  - Constructor functions
  - Prototypes
  - Prototypical Inheritance
  - Property Descriptors
  - How classes use Prototypes

- Module 8: Decorators in TS

  - All about decorators
  - Decorator factories
  - Class members decorators
  - Modifying the prototype
  - Multiple decorators
  - Execution sequence

- Module 9: Advanced concepts and features

  - Type widening
  - Discriminated unions
  - Subtypes and supertypes
  - Typecasting
  - Totality
  - Conditional types

- Module 10, 11, 12: Building a full stack application

  - Frontend: React + TS + Material UI
  - Backend: Node + MySQL + TypeORM
  - Frontend + API Integration: React Query + Context API

### Who should take this course?

- Are you a JS developers? This is for you
- Know a little bit of TS -> advanced TS
- How TS works with other technologies

### What is TS?

- TypeScript is Javascript with syntax for types

TypeScript is a superset of JS with:

- Strict typing
- Editor checks
- Auto complete
- Generics
- OOP features
- Decorators

### Setup dev environments

- Install Node
- Install TypeScript
- Prepare IDE
- Create config file with `tsc --init`

### Your first TS program

```ts
// index.ts

const sum = (a: number, b: number) => {
  return a + b;
};

console.log(sum(1, 2));
```

Transpile TS file with: `tsc index.ts`

See all `tsc` flags with: `tsc --help`

Transpile TS files with specific `tsconfig.json` file.
`tsc -p ./tsconfig.json`

### Setting up Auto Compilation

We can use a better way to compile TS using
a bundle. We could have used Webpack, but since
we want to keep things simple here and focus on
TS, we would use Parcel.

Config Parcel bundler

- init npm project: `npm init -y`
- install parcel: `npm i parcel@2 -D`
- create `index.html`
- create `src` directory for all `ts` stuffs
- create entry point `src/index.ts`
- link `index.ts` in `index.html`, parcel will automatically replace this `ts` file with `js` file for us
- create ts config file with `tsc --init`
- enable flag: `noEmitOnError`
- install `prettier` (reads from docs)
- create `pretter` config file (reads from docs)
- create task runner using npm scripts

  - start: `(npx parcel ./index.html) & npx parcel watch ./index.html`
  - remove `main` property in `package.json` file

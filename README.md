## QUESTION AND ANSWER

## How TypeScript Helps in Improving Code Quality and Project Maintainability

TypeScript improving code quality and project maintainability by following way:

✅ Early Bug Detection – Catches type errors during development, preventing runtime crashes.  
✅ Self-Documenting Code – Clear type annotations improve readability and collaboration.  
✅ Smart Tooling – Autocomplete, refactoring, and error hints speed up development.  
✅ Scalability – Interfaces and strict typing keep large codebases manageable.  
✅ Safer Refactoring – Changing types triggers compile-time errors, reducing hidden bugs.

TypeScript is ideal for teams and long-term projects.

---

## Provide an example of using union and intersection types in TypeScript.

1. Union Types (|)  
   Where any of the mentioned type is valid

```typescript
function printId(id: string | number) {
  console.log(`ID: ${id}`);
}
```

2. Intersection Types (&)
   Merges multiple types into one type.

```typescript
interface User {
  name: string;
}

interface Admin {
  role: string;
}

type SuperUser = User & Admin;

const superUser: SuperUser = {
  name: "Alice",
  role: "Admin",
};
```

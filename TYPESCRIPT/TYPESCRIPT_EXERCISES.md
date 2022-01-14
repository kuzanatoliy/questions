# TypeScript Exercises

### Links

[Sandbox](https://typescript-exercises.github.io)

### Tasks

<details>
  <summary>Task 1</summary>

    export interface User {
      name: string;
      age: number;
      occupation: string;
    }

</details>

<details>
  <summary>Task 2</summary>

    export type Person = User | Admin;

</details>

<details>
  <summary>Task 3</summary>

    export function logPerson(person: Person) {
      let additionalInformation: string;
      if ('role' in person) {
        additionalInformation = person.role;
      } else {
        additionalInformation = person.oc cupation;
      }
      console.log(` - ${person.name}, ${person.age}, ${additionalInformation}`);
    }

</details>

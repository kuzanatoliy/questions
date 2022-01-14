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

<details>
  <summary>Task 4</summary>

    export function isAdmin(person: Person): person is Admin {
      return person.type === 'admin';
    }

    export function isUser(person: Person): person is User {
      return person.type === 'user';
    }

</details>

<details>
  <summary>Task 5</summary>

    export function filterUsers(persons: Person[], criteria: Partial<User>): User[] {
      return persons.filter(isUser).filter((user) => {
        const criteriaKeys = Object.keys(criteria) as (keyof User)[];
        return criteriaKeys.every((fieldName) => {
          return user[fieldName] === criteria[fieldName];
        });
      });
    }

</details>

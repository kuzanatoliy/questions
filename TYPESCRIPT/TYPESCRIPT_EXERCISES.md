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

<details>
  <summary>Task 6</summary>

    const getObjectKeys = <T>(obj: T) => Object.keys(obj) as (keyof T)[];

    export function filterPersons(persons: Person[], personType: 'user', criteria: Partial<User>): User[];
    export function filterPersons(persons: Person[], personType: 'admin', criteria: Partial<Admin>): Admin[];
    export function filterPersons(persons: Person[], personType: string, criteria: Partial<Person>): Person[] {
      return persons
      .filter((person) => person.type === personType)
      .filter((person) => {
        let criteriaKeys = getObjectKeys(criteria);
        return criteriaKeys.every((fieldName) => {
            return person[fieldName] === criteria[fieldName];
        });
      });
    }

</details>

<details>
  <summary>Task 7</summary>

    export function swap<T1, T2>(v1: T1, v2: T2): [T2, T1] {
      return [v2, v1];
    }

</details>

<details>
  <summary>Task 8</summary>

    type OmitType<T> = Omit<T, 'type'>;

    interface PowerUser extends OmitType<User>, OmitType<Admin> {
      type: 'powerUser',
    }

</details>

<details>
  <summary>Task 9</summary>

    export type ApiResponse<T> = {
      status: 'success';
      data: T;
    } | {
      status: 'error';
      error: string;
    };

</details>

<details>
  <summary>Task 10</summary>

    type PCallbackFn<T> = (response: ApiResponse<T>) => void;
    type PResultFn<T> = () => Promise<T>;

    export function promisify<T>(fn: (callback: PCallbackFn<T>) => void): PResultFn<T> {
      return () => {
        return new Promise((resolve, reject) => fn((response) => {
          if(response.status === 'success') {
            return Promise.resolve(response.data);
          }
          else {
            return Promise.reject(response.error);
          }
        }));
      }
    }

</details>

<details>
  <summary>Task 11</summary>

    declare module 'str-utils' {
      type StrUtil = (value: string) => string;

      export const strReverse: StrUtil;
      export const strToLower: StrUtil;
      export const strToUpper: StrUtil;
      export const strRandomize: StrUtil;
      export const strInvertCase: StrUtil;
    }

</details>

<details>
  <summary>Task 12</summary>

    declare module 'stats' {
      type Comparator<T> = (a1: T, a2: T) => number;
      type GetIndex = <T>(input: T[], comparator: Comparator<T>) => number;
      export const getMaxIndex: GetIndex;
      export const getMinIndex: GetIndex;
      export const getMedianIndex: GetIndex;

      type GetElement = <T>(input: T[], comparator: Comparator<T>) => T | null;
      export const getMaxElement: GetElement;
      export const getMinElement: GetElement;
      export const getMedianElement: GetElement;

      export const getAverageValue: <T>(input: T[], getValue: (item: T) => number) => number | null;
    }

</details>

<details>
  <summary>Task 13</summary>

    import 'date-wizard';

    declare module 'date-wizard' {
      const pad: (val: number) => string;

      interface DateDetails {
        year: number;
        month: number;
        hours: number;
        minutes: number;
        seconds: number;
      }
    }

</details>

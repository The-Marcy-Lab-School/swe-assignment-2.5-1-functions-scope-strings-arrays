# Short Responses

For this short response assignment, aim to write a response with the following qualities (your instructor will give you feedback on these areas):
- [] Addresses all parts of the prompt
- [] Accurately uses relevant technical terminology
- [] Is free of grammar and spelling mistakes (double check with grammarly!)
- [] Uses markdown to enhance readability (preview in VS Code with Command/Control + Shift + V)
- [] Is easy to comprehend

For each prompt below, write your response in the space provided. Aim to answer each prompt in 2-5 concise sentences. Make sure to preview your markdown to check how it is rendered before submitting.

## Prompt 1

Using the code block below, explain what it means for a function call to be an "expression that resolves to a value."

```js
const double = (num) => {
  return num * 2;
}

const result = double(5);
```

In your response, make sure to:
1. Explain what an "expression" is
2. Explain how it is determined what value a function call will resolve to
3. Why sometimes function calls resolve to `undefined`.

## Response 1

---

## Prompt 2

Analyze the following code. Draw the callstack and list all variables at the moment when the `getFirstLetter()` function has just been called *for the first time* but has NOT yet returned.

```js
const buildProfile = (firstName, lastName, age) => {
  const fullName = createFullName(firstName, lastName);
  const initials = extractInitials(firstName, lastName);
  const bio = `${fullName} (${initials}) - Age: ${age}`;
  return bio;
}

const createFullName = (first, last) => {
  const fullName = first + " " + last;
  return fullName;
}

const extractInitials = (first, last) => {
  const firstInitial = getFirstLetter(first); // <--- we're in this function call
  const lastInitial = getFirstLetter(last);
  return firstInitial + lastInitial;
}

const getFirstLetter = (name) => {
  // ***draw the callstack at this moment before the return***
  return name[0].toUpperCase();
}

const userProfile = buildProfile("reuben", "ogbonna", 24);
console.log(userProfile); // reuben ogbonna (RO) - Age: 24
```

**Your response should include:**

1. A diagram of the callstack showing all functions currently executing (in order from bottom to top)
2. All variables in each scope with their current values
   1. Use `undefined` for variables not yet defined
   2. Use `waiting` for variables waiting to receive a value from a function call

A template has been provided for you to fill in!

## Response 2

```
Callstack: (top to bottom)
---------------------------
[           ]
[           ]
[           ]
[           ]


Variables by Scope:
---------------------------
Global Scope:
- buildProfile = ?
- createFullName = ?
- extractInitials = ?
- getInitials = ?
- userProfile = ?

buildProfile() scope:
- firstName = ?
- lastName = ?
- age = ?
- fullName = ?
- initials = ?
- bio = ?

createFullName() scope:
- (list any parameters/variables)

extractInitials() scope:
- first = ?
- last = ?
- firstInitial = ?
- lastInitial = ?

getInitials() scope:
- name = ?
```

---

## Prompt 3

These two code snippets look similar but behave differently. Explain what each one prints and WHY they produce different results. Use scope terminology in your explanation.

Example A:

```js
let count = 0;

const incrementA = () => {
  count = count + 1;
  console.log(count);
}

incrementA();
console.log(count);
```

Example B:

```js
let count = 0;

const incrementB = () => {
  let count = count + 1;
  console.log(count);
}

incrementB();
console.log(count);
```

## Response 3

---

## Prompt 4

Explain the concept of "variable shadowing". Use an example to demonstrate this concept.

## Response 4

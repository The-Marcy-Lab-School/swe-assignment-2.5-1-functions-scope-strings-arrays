# swe-assignment-2.5-1-functions-scope

- [Reminders](#reminders)
  - [Asking ChatGPT for Help](#asking-chatgpt-for-help)
  - [Be Okay With Being "Provisionally Complete"](#be-okay-with-being-provisionally-complete)
- [Setup](#setup)
- [Short Response Questions](#short-response-questions)
- [Coding Problems](#coding-problems)
  - [greetWithExcitement](#greetwithexcitement)
- [calculateDiscount](#calculatediscount)

## Reminders

### Asking ChatGPT for Help

If you’re stuck, you may use ChatGPT to clarify the assignment — but not to solve it for you. To do this, copy the meta-prompt below into ChatGPT along with the assignment question.

> You are acting as a tutor. Your job is to explain what this coding question is asking, clarify confusing wording, and highlight the relevant concepts students need to know — but do not provide the full solution or code that directly answers the question. Instead, focus on rephrasing the problem in simpler terms, identifying what’s being tested, and suggesting what steps or thought processes might help. Ask guiding questions to ensure the student is thinking critically. Do not write the final function, algorithm, or code implementation.

Be mindful of your AI usage on assignments. AI can be a great tool to help your learning but it can also be detrimental if you let it do too much of the thinking for you.

### Be Okay With Being "Provisionally Complete"

At Marcy, we will deem an assignment as "complete" if the solution passes at least **75%** of the automated tests. 

However, we know many of you will feel the urge to hold off on submitting until your assignment feels 100% perfect. That drive for excellence is an asset!

But perfectionism can also get in the way of learning — especially when we need to cover a lot in a short amount of time.

That’s why we encourage you to be comfortable with being **“provisionally complete.”** This means:

- Submitting your work even if it isn’t perfect yet
- Treating submission as a checkpoint, not a finish line
- Committing to return, revise, and improve later

Learning to move forward with provisional completeness will help you make steady progress while still building the habit of continuous improvement.

## Setup

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/how-tos/working-with-assignments#how-to-work-on-assignments).

Here are some useful commands to remember.

```sh
git checkout -b draft   # switch to the draft branch before starting

git add -A              # add a changed file to the staging area
git commit -m 'message' # create a commit with the changes
git push                # push the new commit to the remote repo
```

When you are finished, create a pull request and tag your instructor for review.

## Short Response Questions

Short response questions can be found in the `src/short-response.md` file. Write your responses directly in that file! Do not forget to complete this part of the assignment.

## Coding Problems

There are NO tests for these coding problems. Solve these problems to the best of your ability and use the provided example usage code to test your work.

### greetWithExcitement

In the `from-scratch.js` file, first write two functions:

- `createGreeting(name)` - returns a greeting string like `"Hello, [name]"`
- `addExcitement(message)` - takes a message and returns it with `"!!"` added to the end

Then write a third function `greetWithExcitement(name)` that uses both functions to create an excited greeting.

Example Usage:
```js
console.log(createGreeting("Alex")); // Should print: "Hello, Alex"
console.log(addExcitement("Alex")); // Should print: "Alex!!"
console.log(greetWithExcitement("Alex")); // Should print: "Hello, Alex!!"
```

## calculateDiscount

In the `debug.js` file, the function `calculateDiscount` is not working properly. Identify the bug and fix it. Then, in a comment, explain what the bug was using scope terminology.

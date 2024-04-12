## Javascript-important-questions 
# 1. What is the difference between synchronous and asynchronous code? Explain with an example.

#### ANSWER:-)

- `Synchronous Code`:- Executes one task at a time and waits for each task to finish before moving to the next.

```js
console.log("Start");
function greet() {
  return `hey!`;
}
console.log(greet());
console.log("End");
```

- `Asynchronous Code`:- Executes tasks without waiting, allowing other tasks to run while one is in progress.

```js
console.log("Start");
setTimeout(() => {
  console.log("Done"); // this runs later
}, 1000);
console.log("End");
```

---

# 2. What is the use case of call stack?

#### ANSWER:-)

- callstack is basically used for managing at which point of time which code are running.s

---

# 3. What is API? Give example of some web browser APIs.

#### ANSWER:-)

- Application programming Interface(API) is a set of tool for building software and apps.
- Web browser APIs like the DOM (Document Object Model) API for manipulating web pages and the Geolocation API for getting a user's location.

# 4. What does single thread mean?

#### ANSWER:-)

- single thread means that at one point of time single line of code are running.

# 5. What are some of the limitations and advantages of single threaded programming language?

#### ANSWER:-)

- `Advantages`:

```js
- Runs one thing at a time, making it easier to understand
- No complicated issues with things happening at the same time.
```

- `Limitations`:

```js
- If a task takes a long time, the program might stop responding and feel slow.
- Not Good at Multitasking: If there’s a lot happening at once, it can’t handle it efficiently and may lagging.
```

---

# 6. Why call stack is a stack kind of data structure?

#### ANSWER:-)`

```js
- The call stack follows the Last-In, First-Out (LIFO) principle,meaning the last function called is the first one to finish.
- This structure helps manage function calls and returns in an organized way.
```

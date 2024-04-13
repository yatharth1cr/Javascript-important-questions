## Javascript-important-questions 
## 1. What is the difference between synchronous and asynchronous code? Explain with an example.

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

## 2. What is the use case of call stack?

#### ANSWER:-)

- callstack is basically used for managing at which point of time which code are running.s

---

## 3. What is API? Give example of some web browser APIs.

#### ANSWER:-)

- Application programming Interface(API) is a set of tool for building software and apps.
- Web browser APIs like the DOM (Document Object Model) API for manipulating web pages and the Geolocation API for getting a user's location.

## 4. What does single thread mean?

#### ANSWER:-)

- single thread means that at one point of time single line of code are running.

## 5. What are some of the limitations and advantages of single threaded programming language?

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

## 6. Why call stack is a stack kind of data structure?

#### ANSWER:-)

```js
- The call stack follows the Last-In, First-Out (LIFO) principle,meaning the last function called is the first one to finish.
- This structure helps manage function calls and returns in an organized way.
```

## 7. What is the use case of event loop?

#### Answer:-)

```js
- Event loop is basically use to take function from callback queue and handover to callstack for execution.
- it is always taking care of callstack's status that it is empty or not.
- when the callstack will empty it will push the waiting function from callback queue to callstack for execution.
```

## 8. What gets stored in callback queue?

#### Answer:-)

```js
callback queue takes callback from web browser API which marked as completed and store it until code gets executed in callstack.
```

## 9. Write two examples of how you can make network request using XMLHttpRequest

#### Answer:-)

```js
we can make network request using XMLHttpRequest with their method GET,PUT,DELETE & POST
example:-)
let xhr = new XMLHttpRequest()
- xhr.open("GET","URL") 
- xhr.open("POST","URL")
```

## 10. What are the different ways to call function once data is loaded?

#### Answer:-)

```js
```

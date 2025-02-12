# JavaScript Counter without `setInterval`

Without using `setInterval`, try to code a counter in JavaScript. There is a hint at the bottom of the file if you get stuck.

## Example Code

```javascript
let counter = 0;

function incrementCounter() {
    counter++;
    console.log(counter);
    setTimeout(incrementCounter, 1000);
}

incrementCounter();
```

## Explanation

### `let counter = 0;`
This line initializes a variable named `counter` and sets its initial value to 0. The `let` keyword is used to declare a block-scoped variable.

### `function incrementCounter() { ... }`
This function increments the `counter` variable by 1 (`counter++`) and then logs the updated value to the console (`console.log(counter)`). It then uses `setTimeout` to call itself again after 1000 milliseconds (1 second).

### `setTimeout(incrementCounter, 1000);`
The `setTimeout` function calls the `incrementCounter` function after a delay of 1000 milliseconds (1 second). This creates a loop where the `incrementCounter` function is called every second.

### Summary
- **Initialization**: The counter starts at 0.
- **Increment**: Every second, the counter is incremented by 1.
- **Logging**: The updated counter value is printed to the console every second.
- **Loop**: The `setTimeout` function creates a loop by calling the `incrementCounter` function every second.

### Hint
Use `setTimeout` to create a loop that calls the function every second.

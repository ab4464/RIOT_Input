# RIOT_Input
How to create several inputs using RIOT JS

### What kind of html elements and attributes are we using in this application that help us change states? List out at least two examples of how events are working.
The `input` and `button` elements are helping us to access and modify the DOM. In the case of the `input`, it's through the `ref` and value attributes that we can manipulate the user's input while in the case of the `button`, it's the event listener `onclick`, the one that allows us to listen to the user's action and execute a function.

### What is happening in the pre tags? What are pre tags?
The `pre` tag is a pre formatted html tag. In thi case, the `pre` tag is where all the user interaction with the webpage is being printed. 

### How is the app toggle between two states or data? Refer to Button A.
`Button A` is used to trigger the function `toggleStateA`, and because the stateA variable was pre-defined as a Boolean, the function is basically interchanging the Boolean values -TRUE or FALSE- by declaring that everytime that the user clicks, if `stateA` is TRUE, it'll become FALSE and vice versa. That's what the `this.stateA = !this.stateA ` is doing.  

### How are the functions called in riot.js?
In RIOT, the functions are called through event listeners. In this case we have `onclick`, `onkeyup`, `onchange`. Everytime the user interact with the DOM in the specific way is was set in the code (e.g. by clicking, moving the mouse away, etc.), a function is being triggered.

### How are conditionals being used in stateA and stateF?
For `stateA`, because it was initialized as FALSE, when the user clicks it changes to TRUE and the conditional `{ stateA ? "truthy" : "falsy" }` basically states that: if `stateA` is true, then print `truthy`, otherwise print `falsy`.
In the case of `stateF`, all the values where set to FALSE as well. The conditional where use to print `yes` or `no` depending on the Boolean value. The expression `{ stateFPets.alpaca ? "yes" : "no"}` what means is that if `stateFPets` is evaluated to TRUE display `yes`, else display `no`.

How do I feel about the pace of this program so far? The pace of this program worked pretty well for me. At first I was relearning a lot of things, but some of the projects
 really made me work for it. What I like about the projects that we've worked on, is that there is usually a way to make your code better when you're done making them work.

Why are functions a useful tool to organize large programs? If there were no functions, almost everything would be exposed to the global scope. When there is that amount of
publicity in a program, it becomes very easy to recreate a variable that has already been created. Another reason they are useful is once you've created a function and you
know that that function works,that function is reliable and you can safely call it when you need it without having to worry about making errors. Functions can also greatly
reduce the amount of code you have to write, because instead of repeating similar code over and over, you can create a function and use that function wherever it is needed.

What are the different types of scope, and what are some examples? A binding that is created outside of any functions or blocks is located in the global scope, and is
accessible anywhere in the program. Bindings that are created inside a function or block are located inside that function's or block's scope, and are only accessible inside
that scope. These are called local scopes. You can also create functions and blocks within other functions and blocks, which create nested scopes. The inner scope can access
both the outer scope, and the global scope, but neither the outer scope nor the global scope can access bindings within the inner scope. The different scopes are somewhat like a
zoo. The zookeeper should be able to go into any of the cages, but the animals should definitely not be able to roam in and out of their cages.

Here are some examples of how different scopes work:

```
//This is the global scope. The following binding is accessible to anywhere in the program
const inGlobalScope = "I can be accessed anywhere";

const myFunc = function() {
  //This is a local binding
  const inLocalScope = "I can be accessed only between the curly braces";
  //This is a nested function
  const myOtherFunc = function() {
    //This is a local binding
    const InNestedScope = "I can be accessed only between second curly braces";
    //All of these will work
    Console.log(inGlobalScope);
    Console.log(inLocalScope);
    Console.log(inNestedScope);
  }
  //This will not work
  Console.log(inNestedScope);
  //This will
  Console.log(inGlobalScope);
}

//This will not work
Console.log(inLocalScope);
//This will
Console.log(inGlobalScope);
```

## 1
i think it is moving a tad bit fast, the work load with this class and my others is becoming a bit overwhelming to maintain for long periods of time 
especially since i try to work on the weekends aswell im started to feel exhausted.

## 2
Functions can be very useful to make things alot shorter and easier to read. if you were to make a function called jump you could easily call it using jump();
instead of having long lines of code everytime.


## 3
there are two types of scops lexical scope and block scopes. lexical scopes have full insight into the block scopes inside of the function. in a block scoope some things created within the block can escape like var but in a lexical scope nothing can escape

``` 
function zookeeper () {
 let reptiles = 6;
 let mammals = 3;
 const newClosure = () => {
 let reptileLand= reptiles / 2
  console.log(reptileLand);
   
 };
 
  if (reptiles > mammals){
    newClosure();
  
  }
  
}

zookeeper();
```
 if you were to try to call function newClosure after the zoopkeeper brackets it will not work bc its in the lexical scope of zoopkeeper. if you were to try to use the reptileLand anywhere outside of the brackets of newClosure it wouldnt of worked because its in the block scope of newClosure

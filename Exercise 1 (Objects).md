## Solutions Exercise 1

#### 1. Pick a penguin from Wikipedia's List of Fictional Penguins and create an object named myPenguin with properties that represent the information listed in each column on that Wikipedia page (for example: the character's name, origin, and author)
[List of fictional penguins - Wikipedia](https://en.wikipedia.org/wiki/List_of_fictional_penguins).

Solution
```var myPenguin = {
  character: "Tootsie the Penguin",
  origin: "Donald Duck",
  notes: "A baby penguin in the classic 1939 cartoon \"Donald's Penguin\"."
};
``` 

---
#### 2. Use console.log() to print the penguin's name to the console as part of a welcome message, like "Hello, I'm a penguin and my name is [NAME HERE]!"

Solution
```
console.log("Hello, I'm a penguin and my name is " + myPenguin.character + "!");
```
---
#### 3. Write another line of code that adds a new property to your penguin called canFly and set it to false. (Note: Don't modify your penguin-creation code that you wrote above! Do this step in a separate line of code.)


Solution
```
myPenguin.canFly = false;
```
 
---
#### 4. Add a method to your penguin called chirp that prints to the console: "CHIRP CHIRP! Is this what penguins sound like?" (Note: Again, don't modify your previous code! Do this step by writing a new line of code.)

Solution
```
myPenguin.chirp = function() {
  console.log("CHIRP CHIRP! Is this what penguins sound like?");
};
      // TO TEST IT, RUN THIS CODE: myPenguin.chirp();
```
---
#### 5. Add another method to your penguin called sayHello that prints to the console the same message from step 20 above. But this time, be sure to use the mystical, magical, all-powerful this keyword to access your penguin's name, so that way if you change its name later, your method will still work!

Solution
```
myPenguin.sayHello = function() {
  console.log("Hello, I'm a penguin and my name is " + this.character + "!");
};
```
---
#### 6. Next, call your penguin's sayHello() method and make sure that it works! (Hint: if you need an example of what it looks like when you call a method of an object, look at console.log() -- that's how you call the log() method of the console object!)

Solution
```
myPenguin.sayHello();
```
---
#### 7. Without modifying any of your previous code, change the penguin's name to "Penguin McPenguinFace" and then call your penguin's sayHello() function one more time to make sure it still works.

Solution
```
myPenguin.character = "Penguin McPenguinFace";
myPenguin.sayHello();
```
---
#### 8. Write another method called fly, and inside that method, use an if / else statement to print "I can fly!" to the console if your penguin's canFly property is true, or "No flying for me!" if its canFly property is false.

Solution
```
myPenguin.fly = function() {
  if (this.canFly) {
    console.log("I can fly!");
  } else {
    console.log("No flying for me!");
  }
};
```
---
#### 9. Call your penguin's fly() method and make sure it works!

Solution
```
myPenguin.fly();
```

#### 10. Change the canFly property to true -- again, without modifying any of your previous code!

Solution
```
myPenguin.canFly = true;
```
---
#### 11. Now call your penguin's fly() method again and make sure it works as expected!

Solution
```
myPenguin.fly();
```
---
#### 12. Write a for ... in loop to print each key to the console. (Hint: See this page for an example of this special type of loop.
[for...in - JavaScript \| MDN](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Sentencias/for...in))

Solution
```
for (property in myPenguin) {
  console.log(property);
}
```
---
#### 13. Write another for ... in loop to print the value of each key to the console. (Hint: You'll need to use bracket notation to access the values this way, instead of dot notation!)

Solution
```
for (property in myPenguin) {
  console.log(myPenguin[property]);
}
```



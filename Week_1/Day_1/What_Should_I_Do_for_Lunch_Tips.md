```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
  console.log("I don't know what to do!");
    if (hungry === false) {
      console.log("Wait until you are hungry.");
  } else if (hungry === true && availableTime <= 19) {
      console.log("Pick something up and eat it in the lab or in the kitchen where you can get to know your fellow classmates.");
  } else if (hungry === true && availableTime >= 20 && availableTime <= 30) {
      console.log("You deserve a break! You could try a place in Gastown");
  } else if (hungry === true && availableTime > 30) {
      console.log("This is a bootcamp, you should probably reconsider.")
  }
  return whatToDoForLunch;
};

console.log("I'm hungry and I have 20 minutes for lunch.");
whatToDoForLunch(true, 20);
console.log("---");

console.log("I'm hungry and I have 50 minutes for lunch.");
whatToDoForLunch(true, 50);
console.log("---");

console.log("I'm not hungry and I have 30 minutes for lunch.");
whatToDoForLunch(false, 30);
console.log("---");

console.log("I'm hungry and I have 15 minutes for lunch.");
whatToDoForLunch(true, 15);
```

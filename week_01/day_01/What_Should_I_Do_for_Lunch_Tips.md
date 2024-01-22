### Tips

- check for redundant conditions in elses
- Work on your code iteratively – that means in small pieces.
- use constants for messages


```javascript
const NOT_HUNGRY_MSG = "Get back to work!";
const LESS_THAN_20_MSG = "Pick up a snack or grab something you have ready at home";
const BETWEEN_20_AND_30_MSG = "You deserve a break and should take time to cook a tasty meal";
const MORE_THAN_30_MSG = "This is an intense program after all and you should probably reconsider";

const whatToDoForLunch = function(hungry, availableTime) {

  if (!hungry) {
    console.log(NOT_HUNGRY_MSG);
  } else {
    if (availableTime < 20) {
      console.log(LESS_THAN_20_MSG);
    } else if (availableTime >= 20) {
      console.log(BETWEEN_20_AND_30_MSG);
    } else {
      console.log(MORE_THAN_30_MSG);
    }
  }

};
```
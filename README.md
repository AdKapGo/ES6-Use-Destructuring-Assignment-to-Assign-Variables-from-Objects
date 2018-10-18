# ES6-Use-Destructuring-Assignment-to-Assign-Variables-from-Objects
Here is my solution for the 
"ES6: Use Destructuring Assignment to Assign Variables from Objects" challenge on freeCodeCamp.org.  

// Before code is changed
const AVG_TEMPERATURES = {
  today: 77.5,
  tomorrow: 79
};

function getTempOfTmrw(avgTemperatures) {
  "use strict";
  // change code below this line
  const tempOfTomorrow = undefined; // change this line
  // change code above this line
  return tempOfTomorrow;
}

console.log(getTempOfTmrw(AVG_TEMPERATURES)); // should be 79 */

// After code is changed
const AVG_TEMPERATURES = {
  today: 77.5,
  tomorrow: 79
};

function getTempOfTmrw(avgTemperatures) {
  "use strict";
  
  const {tomorrow: tempOfTomorrow} = avgTemperatures;
  
  return tempOfTomorrow;
}

console.log(getTempOfTmrw(AVG_TEMPERATURES)); // should be 79

# ES6-Use-Destructuring-Assignment-to-Assign-Variables-from-Objects
Here is a solution that I came up with for the 
"ES6: Use Destructuring Assignment to Assign Variables from Objects" challenge on freeCodeCamp.org.  

const AVG_TEMPERATURES = {
  today: 77.5,
  tomorrow: 79
};

function getTempOfTmrw(avgTemperatures) {
  "use strict";
  
  const {tomorrow: tempOfTomorrow} = avgTemperatures; // change this line
  
  return tempOfTomorrow;
}

console.log(getTempOfTmrw(AVG_TEMPERATURES)); // should be 79

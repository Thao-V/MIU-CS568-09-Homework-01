# MIU-CS568-09-Homework-01
# Homework 1: JS ES6
## Question 1: What is the output of the following code
```JavaScript
console.log('start...')
function f1(){
  return new Promise((resolve, reject) => {
    console.log(1)
    setTimeout(() => resolve('done'), 1000);
    console.log(2);
  })
}
async function f2(){
  console.log(3);
  let res = await f1();
  console.log(res);
  console.log(4);
}
f2();
console.log('end');
```

## Question 2
Assume that you have a system to manage a human resources of a company.
This system has two classes.
1. People: This class has several properties: name, address, phone, DOB
2. Employee: This class inherits from the class `People`. Besides the inherited attributes, it also has others: position, salary(monthly)
Please implement the followings.
1. Implement the class `People` and `Employee`. Please separate to different files
2. Implement a function to find the employee with the highest salary
3. Implement a function to find the total amount that company pays all employees
## Please submit this homework before 10:00 PM today

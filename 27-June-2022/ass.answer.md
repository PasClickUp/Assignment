Question 1 Solution;

i- Syntax:
Regular function Syntax is more complex than the arrow function syntax.
Below is an example of Regular function:
let name = function (firstName, lastName) {
    let fullName = firstName + lastName;
    return fullName;
}
The above syntax can be easily represented in arrow function as
let name = (firstName, lastName) => firstName + lastName;

ii- Use of "this" Keyword
In a regular function the keyword "this" can be use to call a variable within the function, e.g.
let name = function (firstName, lastName) => {
    firstName: "Abdussomad"
    lastName: "Abdulqodir"
    space: " "
    console.log("My Fullname is "+ this.firstName + space + this.lastName)
}

The above priviledge (i.e. to use the keyword "this")  is limited to regular function alone and can't be in an arrow function.

Question 2 Solution;

Hoisting examples:

i- name()

let name = function (firstName, lastName) {
    let fullName = firstName + lastName;
    return fullName;
}

ii- company()
let company = function (){
    console.log("Code Village Nigeria Limited.")
}

Closure examples:

function printName() {
    let name = "Abdussomad"
    function fullName() {
        let surName = "Abdulqodir"
        let lastname = "Pa-aranti"
        let fullName = `${name} ${surName} ${lastname}`
        return fullName
    }
    return fullName()
}
console.log(printName())


Question 3 Solution;
What are pure & impure functions?
Pure functions are functions that gives the exact result without inclusion of any internal modificatio, While an impure output is an output that gives an alterated result due to the effect  of internal modification of the function.

example of pure function:
function name(firstName, lastName) {
    let fullName = firstName + " " + lastName
    console.log(fullName)
}

name(Abdussomad, Abdulqodir) 
The output of the above function Would be (Abdussomad Abdulqodir) because it was not modified internally.

example of an impure function

function name(firstName, lastName) {
    let fullName = firstName +" " + lastName + " " + "is a student"
    console.log(fullName)
}

name(Abdussomad, Abdulqodir) 
The output of the above function Would be (Abdussomad Abdulqodir is a student) because it has been modied internally..
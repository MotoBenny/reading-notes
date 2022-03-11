# Notes RE JS Classes

### Code Fellows lecture on Classes, inheritance, and data modeling

### Data Modeling

1. constructor functions and prototypes

2. ES6 Classes

  example of a data model (a JS Object)

  person (object)
    Attributes: Hair color, height, weight, location (properties, values tangible things or characters of a person, in this case.)
    behaviors: (verbs): - walk() speak() drive() jump() Methods on the object, things the object can do.

    A person object may contain a few classes, I.E. A child (with different capabilities than an adult class)

- example of how you used to make a class in JS.
``` javascript

// this is the oldschool way of calling a class

const Animal = function(name, legs) { // constructor for animal objects
  this.name = name;
  this.legs = legs;
  this.eat = function () {
    this.isEating = true;
  }
}

Animal.prototype.walk = function () { // a method on the animal objects, to set isWalking to true
  this.isWalking = true;
}

const Dog = function(name, legs) {
  Animal.call(this, name, legs);
}
Dog.prototype = Object.create(Animal.prototype); // this says that the dog object should have all the properties inside the animal constructor. 


let puppy = new Animal('begal', 4); // instantiation of a new animal instance
console.log(puppy); /* the following is displayed in console */ Animal { name: 'begal', legs: 4 }

puppy.walk(); // calling the walk method on the puppy instance. 
console.log(puppy): /* the following is displayed in console */ Animal { name: 'begal', legs: 4, isWalking: true}

puppy.eat();
console.log(puppy): /* the following is displayed in console */ Animal { name: 'begal', legs: 4, eat: [Function], isWalking: true, isEating: true }

let puppy = new Dog('Ellie', 4); // instantiation of a new animal instance

console.log(puppy): /* the following is displayed in console */ Dog { name: 'Ellie', legs: 4, eat: [Function], isWalking: true, isEating: true }
console.log(puppy instanceof Animal); true // Is dog instance of Animal Object? Yes
console.log(puppy instanceof Dog); true // is dog instance of Dog Object? Yes

```

- This is the same functionality using ES6 classes

``` javascript

class Animal { // parent class

  constructor(name, legs) {
    this.name = name;
    this.legs = legs
  }

  walk() { // declaring the walk method, No function or prototype call needed within the class
    this.isWalking = true;
  }

  eat() {
    this.isEating = true;
  }
}


class Dog extends Animal { // subclass
/* because we want to give the dog subclass specific properties unique to it, we call super() with the arguments we would pass to Animal,
then apply the new properties like we otherwise would with a constructor. super calls all the properties of the parent class.  */
  constuctor(name, legs, furType) {
    super(name,legs); // this invokes the constructor on the parent class > creating a version of Animal object
    this.furType = furType;
  }

  speak() { // this method only applies to the Dog subclass
    console.log('wooof!');
  }
}

let rosie = new Animal('rosie', 4);
console.log(rosie); >> Animal { name: 'rosie', legs: 4 }
rosie.walk();
rosie.eat();
console.log(rosie); >> Animal { name: 'rosie', legs: 4, isWalking: true, isEating: true }


let rosie = new Dog('rosie', 4); // instantiating rosie as the Dog subclass of the Animal class
console.log(rosie); >> Dog { name: 'rosie', legs: 4 , 'Short hair'}
rosie.walk();
rosie.eat();
console.log(rosie); >> Dog { name: 'rosie', legs: 4, furType: 'Short hair', isWalking: true, isEating: true }
rosie.speak(): 'wooof!' // only dog subclass can do this.

```
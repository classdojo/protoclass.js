protoclass is a thin class library that helps create, and extend prototypes.

## Example


```javascript


function Animal(name) {
  this.name = name;
}

structr(Animal);

function Cat(name) {
  Cat.superclass.apply(this, arguments);
}

Animal.extend(Cat, {
  meow: function() {
    console.log(this.name + ": meow");
  }
});


console.log(Class.prototype.constructor == Class); // true
console.log(Class.superclass == Animal); // true
consoele.log(Class.name); // Cat


```
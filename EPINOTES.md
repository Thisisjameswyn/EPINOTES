# STANDARD

        function Name () {
          body
        }

# ARROW

        (name) => {
        body
        }
        
        const funct = (name) => {
        body
        }

# FOREACH ARROW

        addJunk(array) {
          array.forEach((thing) => {
            this.stuff.push(thing);
          });
        }

# OBJECT

        let epicodusStudent = {
          firstName: "Charlie",
          lastName: "Bucket",
          level: 1,
          track: ["Ruby","JavaScript","Rails"],
          enrollmentStatus: true   
        };

# CONSTRUCTORS
        
        function Dog(name, colors, age) {
          this.name = name;
          this.colors = colors;
          this.age = age;
        }
        
        let falcor = new Dog("Falcor", ["black"], 4);

# PROTOTYPES

        Dog.protoype.bark = function() {
            //body
        }

# CALLBACK FUNCTION

        function myDisplayer(some) {
          document.getElementById("demo").innerHTML = some;
        }
        
        function myCalculator(num1, num2, myCallback) {
          let sum = num1 + num2;
          myCallback(sum);
        }
        
        myCalculator(5, 5, myDisplayer);

# TEMPLATE LITERAL

        `some text ${jsTieIn}`

# ARRAY DESTRUCTURING

        const myArray = [1,2,3]
        const [firstElement, secondELEMENT, thirdELEMENT] = myArray

# OBJECT DESTRUCTURING

        const obj = {
          color1: "red",
          color2: "blue",
          color3: "yellow",
          description: "Information we don't need",
          anotherProp: "We don't need this info, either"
        };
        
        const { color1, color2, color3 } = obj; //keep names of properties
        
        const { color1: red, color2: blue } = obj;

# JS CLASS

        class Triangle {
          constructor(side1, side2, side3) {
            this.side1 = side1;
            this.side2 = side2;
            this.side3 = side3;
          }
        
          checkType() {
            //Function body goes here.
          }    
        }

# TEST SYNTAX

        import Rectangle from '../src/js/rectangle.js';
        
        describe('Rectangle', () => {
        
          test('should correctly create a rectangle object using two sides', () => {
            const rectangle = new Rectangle(3,5);
            expect(rectangle.side1).toEqual(3);
            expect(rectangle.side2).toEqual(5);
          });
        });

# IMPORT/EXPORT

        const Triangle = require('./triangle.js').triangleModule;
        
        export function Triangle(side1, side2, side3) {
          this.side1 = side1;
          this.side2 = side2;
          this.side3 = side3;
        }
        
        import { Triangle } from './triangle.js';
        
# EXPORT SINGLE ITEM

        export default function Triangle(side1, side2, side3) {
        }
        
        import Triangle from './triangle.js';

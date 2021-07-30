# Using-JavaScript-Class-for-Area-of-Rectangle
Illustration of JavaScript Class Using Area Calculation


<pre>
<code>
// In this example, we are calculating Area of a triangle
//  We explain this through using JavaScript Class, Object constructors and Methods

class AreaOfRectangle {

    constructor (length, width, texture, color){
        this.length = length;
        this.width = width;
        this.texture = texture;
        this.color = color;
    }
    // In the Below sections, three methods are created, that will be applied to accomplish key tasks in the class AreaOfRectangle

    // Creating a Method for calculating the Area of teh Rectangle
    getArea () {
        return this.width * this.length;
    }
    // Method to get the square of length and square of width
    getLengthSquare (){
        return this.length * this.length;
    }
    getWidthSquare (){
        return this.width * this.width;
    }
    // Creating a Method for providing the description of the Rectangles
    printDescription () {
        console.log(`I am a Rectangle of Length ${this.length} cm X and width ${this.width} cm, with Color ${this.color} and Texture ${this.texture}`);
    }
    // Creating a Method for giving a Description of the colors of the Rectangles
    getColors () {
        console.log(`This Rectangle of ${this.length} cm and ${this.width} cm is of Color ${this.color}`);
    }
    
    }
    // In this section, we are creating three rectangle objects
    let Rectangle1 = new AreaOfRectangle(2, 50, 'Smooth', 'Red');
    let Rectangle2 = new AreaOfRectangle(12, 12, 'Rough', 'Blue');
    let Rectangle3 = new AreaOfRectangle(10, 50, 'Normal', 'Yellow')
    
    // calling colors function
    Rectangle1.getColors();
    Rectangle2.getColors();
    Rectangle3.getColors();
    
    
    /*
    
    RESULTS WILL BE
    
    This Rectangle of 2 cm and 50 cm is of Color Red
    This Rectangle of 12 cm and 12 cm is of Color Blue
    This Rectangle of 10 cm and 50 cm is of Color Yellow
    
    */
    
    Rectangle1.printDescription();              // call the function printdescription here
    Rectangle2.printDescription();
    Rectangle3.printDescription();
    
    
    /*
    ====RESULTS WILL BE;
    
    I am a Rectangle of Length 2 cm X and width 50 cm, with Color Red and Texture Smooth
    I am a Rectangle of Length 12 cm X and width 12 cm, with Color Blue and Texture Rough
    I am a Rectangle of Length 10 cm X and width 50 cm, with Color Yellow and Texture Normal
    
    
    */
    console.log(Rectangle1.length);         // 2
    console.log(Rectangle1.width);          // 50
    console.log(Rectangle1.getArea());      // 1000
    console.log(Rectangle2.getArea());       // 144      
    console.log(Rectangle3.getArea());      // 1500


    console.log(`The Square of ${Rectangle1.length} is: `, Rectangle1.getLengthSquare());
    console.log(`The Square of ${Rectangle2.length} is:  `, Rectangle2.getLengthSquare());
    console.log(`The Square of ${Rectangle3.length} is: `, Rectangle3.getLengthSquare());

  </code>
</pre>

    // RESULTS WILL BE AS FOLLOWS

<pre>
  <code>


    /*

This Rectangle of 2 cm and 50 cm is of Color Red
This Rectangle of 12 cm and 12 cm is of Color Blue
This Rectangle of 10 cm and 50 cm is of Color Yellow
I am a Rectangle of Length 2 cm X and width 50 cm, with Color Red and Texture Smooth
I am a Rectangle of Length 12 cm X and width 12 cm, with Color Blue and Texture Rough
I am a Rectangle of Length 10 cm X and width 50 cm, with Color Yellow and Texture Normal
2
50
100
144
500
The Square of 2 is:  4
The Square of 12 is:   144
The Square of 10 is:  100

    */
  </code>
</pre>

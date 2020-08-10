# Python Turtle - Flower Shape

1. To begin using Turtle in Python, you need to import the Turtle library. So type *import turtle*
2. You will need to give your Turtle a name and this can be done by assigning a variable to it. e.g. Call it 'line' by writing: 
  *line = turtle.Turtle()

3. Now you can create your lines. For example *bob.forward(100)* .This creates a straight line that moves 100 units forward.
4. You can change directions, such as *bob.right(90)*. This would change the direction of the next line by 90 degrees to the right.
5. You can start off by trying to create a parallelogram. 
   I used a loop that loops twice so 4 lines are created instead of 2, to create the first parallelogram.

**Add these lines next**
*for i in range(2):
   line.forward(100)
   line.right(60)
   line.forward(100)
   line.right(120)
   
 5. Next, in order to create an identical parallelogram but in another direction, you will need to put the existing loop inside another loop.
 6. Above the *for i in range(2)* line, place this line: *for i in range(10)* and indent everything below it. This will create 10 parallelograms 
    altogether, instead of just 1.
 7. To make each parallelogram go in a slightly different direction, add this line below the second *for* loop:  *line.right(36)*
 
 8. To finish the code, write *turtle.done()* at the end.
 
 **The code should look like this:**
 
    import turtle
    line = turtle.Turtle()
    
    line.color("blue")  #These 3 lines aren't needed. This gives the line a colour chosen by you.
    turtle.Screen().bgcolor("grey")  #This gives the background a colour
    line.speed(7)  #This specifies how fast the lines will be drawn

    for i in range(10):
        for i in range(2):
            line.forward(100)
            line.right(60)
            line.forward(100)
            line.right(120)
        line.right(36)  

    turtle.done()
    
  

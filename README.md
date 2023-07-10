# Maze Runner

To create a Maze Runner in which we have to collect all of the 4 coins inside the maze and solve the maze in as little time as possible using a graphics library in C.


## Working

When the user starts the game, the program displays the maze and all the coins. The exit gate is closed and only opens after all the 4 coins have been collected, this is achieved by using a counter which checks if the current position is equal to the coin position, if true then it increments the coin counter, and the same is reflected on screen.

For input, ASCII values of arrow keys were compared with the input values. If the input was equal to the ASCII values of up, down, right or left keys, then the position would be changed if it is valid.

A position is valid if it does not cross the maze walls. This is done by adding +10 to the current position in the direction of input. If the new position is not intersecting the maze walls(boundary) then the current position is changed to a new position. Position is checked by comparing the New Position color with boundary color. If it matches that means that the new position is invalid so a message is displayed saying “INVALID INPUT” and input is taken again using getch() function.

Input is taken using a while loop which terminates when the user reaches the exit after collecting all 4 coins.

Maze is drawn using the line() function of the graphics.h library.

## Library used

1. graphics.h

    C graphics using graphics.h functions or WinBGIM (Windows 7) can be used to draw different shapes, display text in different fonts, change colors and many more. 
    Using functions of graphics.h in Turbo C compiler you can make graphics programs, animations, projects, and games. You can draw circles, lines, rectangles, bars and many other geometrical figures. 
    You can change their colors using the available functions and fill them. Following is a list of functions of graphics.h header file. Every function is discussed with the arguments it needs and its description.

2. time.h 

    The time.h header defines four variable types, two macro and various functions for manipulating date and time.




## Function Used

1. Cleardevice: 

    cleardevice function clears the screen in graphics mode and sets the current position to (0,0). Clearing the screen consists of filling the screen with current background color.

2. Closegraph: 

    Closegraph function closes the graphics mode, deallocates all memory allocated by the graphics system and restores the screen to the mode it was in before you called initgraph
    .
3. Getcolor: 

    Getcolor function returns the current drawing color. Declaration : int getcolor();

4. Getpixel:

    Getpixel function returns the color of the pixel present at location(x, y).

5. Line: 
    
    Line function is used to draw a line from a point(x1,y1) to point(x2,y2) i.e. (x1,y1) and (x2,y2) are end points of the line. The code given below draws a line. Declaration: void line(int x1, int y1, int x2, int y2);

6. Outtextxy: 

    Outtextxy function displays text or string at a specified point(x,y) on the screen. Declaration: void outtextxy(int x, int y, char *string);

7. Circle: 

    Circle function is used to draw a circle with center (x,y) and third parameter specifies the radius of the circle. The code given below draws a circle .Declaration: void circle(int x, int y, int radius);

8. Putpixel: 

    Putpixel function plots a pixel at location (x, y) of specified color. Declaration: void putpixel(int x, int y, int color);

9. Floodfill: 

    Floodfill function is used to fill an enclosed area. Current fill pattern and fill color is used to fill the area. (x, y) is any point on the screen. If (x,y) lies inside the area then inside will be filled otherwise outside will be filled. Border specifies the color of the boundary of the area. To change fill pattern and fill color use setfillstyle.

10. Rectangle: 

    Rectangle function is used to draw a rectangle. Coordinates of left top and right bottom corner are required to draw the rectangle. left specifies the X-coordinate of top left corner, top specifies the Y-coordinate of top left corner, right specifies the X-coordinate of right bottom corner, bottom specifies the Y-coordinate of right bottom corner.
## Variables Used

1. size_t

    This is the unsigned integral type and is the result of the sizeof keyword.

2. clock_t

    This is a type suitable for storing the processor time.

3. time_t

    This is a type suitable for storing the calendar time.

4. struct tm

    This is a structure used to hold the time and date.


## Images

![one](https://pasteboard.co/JarVH2RZ0fVZ.jpg)

![two](https://pasteboard.co/ThBFBhVnr4bz.jpg)

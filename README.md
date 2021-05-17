# Figures
Given: class Point, abstract class Figure,
 skeletons of classes Triangle, Quadrilateral, Circle.

Make Triangle, Quadrilateral, Circle extend Figure class.

Implement methods in Triangle, Quadrilateral, Circle

Given a class Point, an abstract class Figure,
skeletons of classes Triangle, Quadrilateral, Circle, implement the following.
Make Triangle, Quadrilateral, Circle extend Figure class.
Implement methods in Triangle, Quadrilateral, Circle:


constructors with following parameters:


Triangle - three vertices (points) as parameters.

Quadrilateral - four vertices (points) as parameters.

Circle - point of the center and double value of the radius.

All the input datasets in tests are guaranteed to form a non-degenerative figures.
For Quadrilaterals, it is guaranteed that all test datasets would form a convex quadrilaterals.


public double area()
Return the area of the figure.
Note: Convex quadrilaterals are divided into two triangles by any of their diagonals.


public String pointsToString()
Return a String value in following formats:


Triangle -

Format: (a.x,a.y)(b.x,b.y)(c.x,c.y)

Example: (0.0,0.0)(0.1,5.8)(7.0,7.0)




Quadrilateral -

Format: (a.x,a.y)(b.x,b.y)(c.x,c.y)(d.x, d.y)

Example: (0.0,0.0)(0.0,7.1)(7.0,7.0)(7.0,0.0)




Circle -

Format: (center.x,center.y)

Example: (0.0,0.6)




Note:: you may benefit from implementing toString() in the Point class


public String toString()
Return a String value in following formats:


Triangle -

Format: Triangle[(a.x,a.y)(b.x,b.y)(c.x,c.y)]

Example: Triangle[(0.0,0.0)(0.1,5.8)(7.0,7.0)]




Quadrilateral -

Format: Quadrilateral[(a.x,a.y)(b.x,b.y)(c.x,c.y)(d.x, d.y)]

Example: Quadrilateral[(0.0,0.0)(0.0,7.1)(7.0,7.0)(7.0,0.0)]




Circle -

Format: Circle[(center.x,center.y)radius]

Example: Circle[(0.0,0.6)4.5]




Note: you may use default implementation given in the Figure class, when it suits a case well.


public Point leftmostPoint()
Return a leftmost point of the figure: the one having the least X coordinate.
If there are many leftmost points, return any of them.


Hints:

Degeneracy reference
Convex quadrilateral reference
Triangle area reference
Circle area reference
Quadrilateral area reference


Examples
You may use Main class to try your code.
There are some examples below.

Sample code:
...
double area = new Triangle(new Point(0,0), new Point(3, 0), new Point(0, 4)).area();
System.out.println(area);
Output:
6

Sample code:
...
double area = new Quarilateral(new Point(1,0), new Point(2, 1), new Point(1, 2), new Point(0, 1)).area();
System.out.println(area);
Output:
2

Sample code:
...
double area = new Circle(new Point(1,1), 3).area();
System.out.println(area);
Output:
28.274333882308138

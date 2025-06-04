## Name : Aadhithya D
## Reg No : 212222220001
# EX 3 : Circle Drawing Algorithm

**AIM :**

To  implement the Bresenham’s  algorithm for circle using a c coding.


**ALGORITHM :**

Step 1 : Start.
    
Step 2 : Initialize the graphics header files and functions.
   
Step 3 : Declare the required variables and functions.
 
Step 4 : Get the co-ordinates and radius of the circle.

Step 5 : Draw the circle using the algorithm.

Step  6 : Display the output.
  
Step 7 : stop.

**Program :**
initgraph(&gd, &gm, "C:\\Turboc3\\BGI");  // Update path based on your setup

printf("Enter the Radius Value:\n");
scanf("%d", &radius);
printf("Enter the xcenter and ycenter Values:\n");
scanf("%d %d", &xcenter, &ycenter);

x = 0;
y = radius;
p = 1 - radius;

plotpoints(xcenter, ycenter, x, y);

while (x < y) {
    x++;
    if (p < 0) {
        p += 2 * x + 1;
    } else {
        y--;
        p += 2 * (x - y) + 1;
    }
    plotpoints(xcenter, ycenter, x, y);
}

getch();
closegraph();
return 0;



**Output :**

![437692095-1c182f48-ccc7-4758-b9cb-2217e228ee7d](https://github.com/user-attachments/assets/422bcff3-befc-49a0-a5a2-8d1edc89c403)


**Result :**

To implement the Bresenham’s algorithm for circle using a c coding verified successfully.

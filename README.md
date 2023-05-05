Download Link: https://assignmentchef.com/product/solved-ece210-homework-5-cell-arrays-classes-chars-and-dataset
<br>
We will review some of the advanced data types in MATLAB, such as cell arrays, classes, chars, as well as dataset importing in MATLAB. You will be importing in the fisheriris dataset and encapsulating it in classes.

1. Take a minute to research the fisheriris dataset (it’s a popular dataset, you might see it again in an ML class).

Load in the fisheriris dataset with load fisheriris. You should obtain (in your workspace) a 150×4 matrix called meas, as well as a 150×1 cell array called species. The i-th row in species corresponds to the i-th row in meas.

(a)    Create a class Flower in its own file. (Look up the syntax for userdefined classes!) You should have the following properties:

PropertyTypepetalWidthdoublepetalLengthdoublesepalWidthdoublesepalLengthdoublespecieschar (array)Note that you do not need to specify the data type of the properties when you are declaring a class; the following properties are just here to impress on you what type of properties you would be expecting.

(b)    Create a constructor for Flower. It should take in four doubles and a character array corresponding, in order, to the five properties of your class.

1

(c)    Now, import the entries from from meas and species into a 150 × 1 cell array of Flower instances. You can use a for loop to import the entries, or look up a way to vectorize the initialization (although the vectorization may take a few extra lines in this case).

Note that the name of the species are stored in a cell array; make sure to extract the character array from the cell before storing them in the Flower instances.

(d)   Create a method getSWidth in the Flower class that returns the sepal length of the object. Use this on the 51st Flower in your cell array, and verify that it is the correct value against the corresponding entry in meas (i.e., using ==).

(e)    Create another method called report in the Flower class that will print out details about the object on the command window. This function takes no arguments and returns nothing. It should print out a statement of the following form, but with the correct values of the object’s properties:

The length and width of its sepal are 5.1cm and 3.5cm respectively, while the length and width of its petal are 1.4cm and 0.2cm respectively. It belongs to the setosa species.

Demonstrate that this function works on the 51st Flower object.

2
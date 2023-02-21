# anneenaissance

The provided Swift code defines several functions that are demonstrated with test cases.

- saluer(prenom:) function takes in a parameter named prenom of type String and prints it using print function. It does not return anything.
- calculerAge(anneeNaissance:) function takes in a parameter named anneeNaissance of type UInt and returns an UInt value which is the difference between the current year 2019 and the provided year of birth.
- calculerAgeDe(nom:anneeNaissance:) function takes in two parameters, a nom of type String and an anneeNaissance of type UInt. It returns a tuple of type (String, UInt) containing the provided nom and the age calculated from the anneeNaissance parameter.
- maFonction is a variable of type (String, UInt) -> (String, UInt) that references calculerAgeDe function. It can be used to call calculerAgeDe function.
- calculerMinMax is a variadic function which takes a list of integers as a parameter. It returns a tuple with three values; the minimum value of the list, the sum of the values, and the average of the values.

The code tests the functions by calling them with appropriate parameters, and prints the results. It first calls the calculerAgeDe(nom:anneeNaissance:) function with parameters "John" and 1970, then prints the tuple's elements using their indices. Next, it assigns the reference of the calculerAgeDe function to the variable maFonction, and calls it with parameters "Sylvain" and 1980, again, printing the tuple's elements using their indices.

After that, the code computes the maximum value in an array using a loop and prints it. Then, it calls the calculerMinMax function with a few test cases and stores the result in data. Finally, it calls calculerMinMax with more integers using the maFonction2 variable, which was assigned the same reference as calculerMinMax with a different signature. It prints the first element of the tuple data2 which contains the minimum value of the input values.

# Grade-Determination
A-F grade determaination
# Input statements
studentName = str(input("<Enter the student's name> "));
test1 = float(input("<Enter first test score #1 of the student> "));
test2 = float(input("<Enter first test score #2 of the student> "));
test3 = float(input("<Enter first test score #3 of the student> "));
test4 = float(input("<Enter first test score #4 of the student> "));
test5 = float(input("<Enter first test score #5 of the student> "));

#============================================================================================
#Calucalations / processing
sumTest = test1 + test2 + test3 + test4 +test5;
testAvg = sumTest / 5
letterGrade = "";

#============================================================================================
# Output Statements
print();
print( "TEST RESULTS FOR " + studentName + ":");
print( "-" * 60);
print( "Test #1 = " + format(test1, "6.2f") + "%");       
print( "Test #2 = " + format(test2, "6.2f") + "%");
print( "Test #3 = " + format(test3, "6.2f") + "%");
print( "Test #4 = " + format(test4, "6.2f") + "%");
print( "Test #5 = " + format(test5, "6.2f") + "%");
print( "-" * 60);
print("The sum of all the test scores = " + format (sumTest, "7.2f"));
print("The average of the test scores = " + format(testAvg, "7.2f") +"%");
print( "-" * 60);
#============================================================================================
#Sequential IF statements to determine a letter grade based on the calculated test average.

if (testAvg <=100) and (testAvg >= 90):
    letterGrade = "A";
if (testAvg <=89.99) and (testAvg >= 87):
    letterGrade = "B+";
if (testAvg <=86.99) and (testAvg >= 80):
    letterGrade = "B";
if (testAvg <=79.99) and (testAvg >= 77):
    letterGrade = "C+";
if (testAvg <=76.99) and (testAvg >= 70):
    letterGrade = "C";
if (testAvg <=69.99) and (testAvg >= 67):
    letterGrade = "D+";
if (testAvg <=66.99) and (testAvg >= 60):
    letterGrade = "D";
if (testAvg <=59.99) and (testAvg >= 0):
    letterGrade = "F";
#===============================================================================================
# Print letter grade
print("=" *60);
print(studentName + " Earned a letter grade of an/a " + letterGrade);
print("=" *60);
#===============================================================================================
# End Program 

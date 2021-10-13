Brief introduction: This is an exercise from the book "Data Structures and Algorithms Using Python", author Rance D. Necaise. First, we extract data from a text file. Five fields of the record: idNum, firstName, lastName, classCode and gpa. Each field is stored on a seperate line.

10015 
John 
Smith
2
3.01
10334
Jane
Roberts
4
3.81

In studentfile.py module 
-The constructor initializes an instance of the class by creating two attributes, one to store name of the text file and the other to store a reference to the file object after it's opened.
- open() method is responsible for opening the input file 
- close() method is to close the file after the records are extracted.
- fetchAll() method builds and returns a list of StudentRecord objects. This is done by repeatedly calling the fetchRecord() method
- fetchRecord() method: this is where actual extraction from the record in the text is handled.

The Student File Reader ADT provides a framework that can be used to extract any type of records from a text file. The only change required would be in the fetchRecord() method to create the appropriate storage object and to extract the data from the file in the given format.

The studentreport.py program consists of two functions: printReport() and main().
- main() uses an instance of the StudentFileReader class to extract student record into a list. The list of records is then sortd in the ascending order based on idNum 
- printReport() is used to produce a report by passing the sorted list as an inpuy.

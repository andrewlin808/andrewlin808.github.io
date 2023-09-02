---
layout: project
type: project
image: img/ICS 212 Database Project Image.jpg
title: "Record Database"
date: 2022
published: true
labels:
  - C/C++
  - ICS 212
  - Database
summary: "A database project from ICS 212 to store and retrieve banking customer's information."
---


As a two-part final project for my ICS 212 class, all students, on their own, were to design a program that can store and retrieve banking customer' information through a terminal user interface, using the C (part 1) and C++ (part 2) programming language. Each banking customer have their (1) account number (int), name (char[]), address (char[]), and a pointer (record*) to a next entry stored as a structure called record in C/C++. The C code was later converted to C++ code as we learned about the C++ programming language in class as part 2 of the project.

The follow C code shows the header file for the strcture record that stores banking customer's information:
```c
#ifndef RECORD_H
#define RECORD_H

struct record
{
    int               accountno;
    char              name[30];
    char              address[50];
    struct record*    next; 
};



#endif
```
The follow C code shows the user interface in the terminal window for adding a banking customer's record into the database:

```
Select one of the options below:
add: add a new customer record
printall: print all existing record(s) of customers
find: find record(s) of an existing customer
delete: delete record(s) of an existing customer
quit: exit the program
Awaiting input...
a


Add a new record:

Enter the account number to find: 
1234

Enter the account name: 
andrew lin
Enter the account mailing address: (type '!' at the end to indicate the end of the address)
2555
Dole  
98 6822!

Adding new record to database: 

Record with account #1234 has been added to the database!

Select one of the options below:
add: add a new customer record
printall: print all existing record(s) of customers
find: find record(s) of an existing customer
delete: delete record(s) of an existing customer
quit: exit the program
Awaiting input...
p

Print all records:

Record Entry #1
Account #1234
Name: andrew lin
Address:
2555
Dole
96822

---End-of-Records-List---
```


You can learn more about my project here [source code]: (https://manoa.hawaii.edu/news/article.php?aId=2857).

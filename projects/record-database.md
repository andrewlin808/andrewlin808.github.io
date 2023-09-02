---
layout: project
type: project
image: img/ICS 212 Database Project Image.jpg
title: "Record Database"
date: 2022
published: true
labels:
  - C++
  - ICS 212
  - Database
summary: "A database project from ICS 212 to store and retrieve banking customer's information."
---


As a two-part final project for my ICS 212 class, all students, on their own, were to design a program that can store and retrieve banking customer' information through a terminal user interface, using the C (part 1) and C++ (part 2) programming language. Each banking customer have their (1) account number (int), name (char[]), address (char[]), and a pointer (record*) to a next entry stored as a structure called record in C/C++.

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

You can learn more about my project here [source code]: (https://manoa.hawaii.edu/news/article.php?aId=2857).

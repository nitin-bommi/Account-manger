# Account Manager

[![Build Status](https://travis-ci.org/Nitin1901/Account-manger.svg?branch=master)

### How the code is managed

The above code is divided into different functions which include,
+ `welcome()`
+ `home(address)`
+ `login()`
+ `register()`
+ `validate(address, password)`
+ `addToDatabase(address, password)`
+ `transfer(address)`

The `welcome()` function is called iniially and then different functions are returned according to the instructions.

## Getting started 

### Libraries used:-
+ `ipywidgets` - To create basic widgets. [Click here](https://ipywidgets.readthedocs.io/en/latest/).
+ `IPython.display` - To displaye the created widgets. [Click here](https://ipython.org/ipython-doc/dev/api/generated/IPython.display.html).
+ `pymongo` - To establish a connection to the MongoDB server. [Click here](https://github.com/Nitin1901/MongoDB-cheatsheat).
+ `urllib` - To enter the cluster credentials. [Click here](https://docs.python.org/3/library/urllib.html).

### Establising a connection.
The steps to establish a secure connection are given [here](https://github.com/Nitin1901/MongoDB-cheatsheat).
1) Get access to the cluster.
2) Access the database.
3) Access the collection and make changes on it.

### Calling the funstions.
When the code is run, initially, `welcome()` function is called manually.

Later on, different functions are returned based on a particular condition as, 
```python
if cond1:
  return func1()
else:
  return func2()
```

### Creating and using the widgets.
Only few widgets are used here
+ `Button`
+ `Text`
+ `Password`

These methods have parameters which modify them.

### Affecting the database.
Any change to the collection in any row is updated directly to the database.

Like,
```python
collection.update_one(myquery_debit, newvalues_debit)
```

### Conclusion.
This code makes use of database to store and access accounts.

We can either 
+ Create a new account in the database

or
+ Modify the account

As the code makes use of databse, we can store info of many people.
As the code progresses according to conditions, it is secure to use.

We can implement this in many __Banking Applications.__




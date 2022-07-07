# Understanding Interactive Zeppelin Forms in Oracle Machine Learning
## *Oracle Machine Learning Certification Series*

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/puzzle.jpg)

source: iStock

Be familiar with the 3 interactive Zeppelin forms and the scripting syntax for the certification.  You may need to identify the type of form by the syntax given.

Here are examples below for each form.

## Select Form:

The Select Form allows you to select input values from a list of values, and dynamically
retrieve the selected values as defined in the paragraph.

Script Syntax: ${formName=defaultValue,option1|option2...}

**Example 1 (See Oracle Machine Learning Documentation):** 
```
%sql

SELECT * FROM ALL_OBJECTS WHERE OBJECT_TYPE = '${OBJ=INDEX,INDEX|TABLE|VIEW|SYNONYM}';
```
![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/select.png)

In this example:
*	The form name is obj
*	The list of available values are INDEX, TABLE, VIEW, SYNONYM.
*	The table name is ALL_OBJECTS
*	The column name is OBJECT_TYPE

Select any values from the drop-down list in the obj form. The selected value will
be retrieved in the OBJECT_TYPE column in the ALL_OBJECTS table.

**Example 2:**
```
%sql

SELECT * FROM IRIS WHERE SPECIES = '${OBJ=INDEX,virginica|setosa|versicolor}';
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/select_iris.png)

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/select_form_bob.png)

**Section Notes:** 
*	The form name can be changed to a value meaningful for you.  For example, you can call the form BOB.
* The available list of values in this form are the iris species within the table (virginica, setosa, versicolor)
*	The table name is the name of the table you are using.  In my example, I have the IRIS dataset as a table in my ADB user schema.
*	The column name is SPECIES.

##Text Form: 

The Text Input form allows you to dynamically retrieve values as defined in the
notebook.

Script Syntax: ${formName}

**Example 1 (See Oracle Machine Learning Documentation):**
```
%sql

SELECT * FROM ALL_OBJECTS WHERE OBJECT_TYPE = '${OBJ}';
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/text.png)

In this example:
•	The form name is obj
•	The table name is ALL_OBJECTS
•	The column name is OBJECT_TYPE

Example 2:
```
%sql

SELECT * FROM IRIS WHERE SPECIES = '${OBJ}';
```
![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/text_iris.png)

Section Notes: 
•	The form name can be changed to a value meaningful for you.  For example, you can call the form BOB.
•	The table name is the name of the table you are using.  In my example, I have the IRIS dataset as a table in my ADB user schema.
•	The column name is SPECIES.
•	To retrieve a list of values from the table, select a species name.

## Check Box Forms:

The Check Box Form supports multiple selection of inputs in a paragraph. The inputs
are available as check box options in the notebook.

${checkbox:formName=defaultValue1|defaultValue2...,option1|option2...}

Example 1 (See Oracle Machine Learning Documentation): 
```
%sql

SELECT ${checkbox:whichcolumn=OWNER|OBJECT_TYPE, OWNER|OBJECT_NAME|OBJECT_TYPE|CREATED|STATUS} FROM ALL_OBJECTS WHERE OBJECT_TYPE IN ('VIEW',
'TABLE', 'INDEX', 'SYNONYM');
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/checkbox.png)

In this example:
•	The Check Box form is WhichColumn
•	The multiple selection options available in the check boxes are OWNER,
OBJECT_NAME, OBJECT_TYPE, CREATED, and STATUS
•	The fields OWNER and OBJECT_TYPE are defined as default
•	The table name is ALL_OBJECTS
•	The columns that are configured for display are OWNER, OBJECT_NAME,
OBJECT_TYPE, CREATED, and STATUS

Example 2:
```
%sql

SELECT ${checkbox:whichcolumn=ID|SPECIES,SEPAL_LENGTH|SEPAL_WIDTH|PETAL_LENGTH| PETAL_WIDTH|SPECIES|ID} FROM IRIS WHERE SPECIES IN ('virginica','setosa','versicolor');
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/checkbox_iris.png)

Section Notes: 
*	The Check Box form is WhichColumn
*	The multiple selection options available in the check boxes are SEPAL_LENGTH, SEPAL_WIDTH, PETAL_LENGTH, PETAL_WIDTH, SPECIES, and ID 
*	The fields ID and SPECIES are defined as default
*	The table name is IRIS


*Sourcing:*
*Content sourced from Oracle Machine Learning Documentation.*


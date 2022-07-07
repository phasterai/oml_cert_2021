# Output Formats Available with Oracle Machine Learning
## *Oracle Machine Learning Certification Series*

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/puzzle.jpg)

source: iStock

Output formats are testable material on the Oracle Machine Learning certification. I am excerpting the output formats from Oracle documentation because they are significant for the exam, and it is easier to see them in one list. You can find more information about output formats in the Oracle Machine Learning Documentation. Refer to section Output Formats Supported by SET SQLFORMAT Command.

Let’s see what the output formats are and how to invoke them.  First, look at the output from a SELECT statement performed in the Scratchpad without SET SQLFORMAT. 

<image0.png> [none.png]

Now, add SET SQLFORMAT to our script and observe the output. To use these output formats, you must include the prefix %script.

**CSV:** The CSV format produces standard comma-separated variable output, with string values enclosed in double quotes. The syntax is: 
```
%script 
SET SQLFORMAT CSV
```
![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/csv.png)

**HTML:** The HTML format produces the HTML for a responsive table. The content of the table changes dynamically to match the search string entered in the text field. The syntax is: 

```
%script 
SET SQLFORMAT HTML
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/html.png)

**XML:** The XML format produces a tag based XML document. All data is presented as CDATA tags. The syntax is: 

```
%script 
SET SQLFORMAT XML
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/xml.png)

**JSON:** The JSON format produces a JSON document containing the definitions of the columns along with the data that it contains. The syntax is: 

```
%script 
SET SQLFORMAT JSON 
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/json.png)

**ANSICONSOLE:** The ANSICONSOLE format resizes the columns to the width of the data to save space. It also underlines the columns, instead of separate line of output. The syntax is: 

```
%script 
SET SQLFORMAT ANSICONSOLE 
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/ansiconsole.png)

**INSERT:** The INSERT format produces the INSERT statements that could be used to recreate the rows in a table. The syntax is: 

```
%script 
SET SQLFORMAT INSERT 
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/insert.png)

**LOADER:** The LOADER format produces pipe delimited output with string values enclosed in double quotes. The column names are not included in the output. The syntax is: 

```
%script
SET SQLFORMAT LOADER
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/loader.png)

**FIXED:** The FIXED format produces fixed width columns with all data enclosed in double-quotes. The syntax is: 

```
%script 
SET SQLFORMAT FIXED
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/fixed.png)

**DEFAULT:** The DEFAULT option clears all previous SQLFORMAT settings, and returns to the default output. The syntax is: 

```
%script 
SET SQLFORMAT DEFAULT
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/default.png)

**DELIMITED** — The DELIMITED format allows you to manually define the delimiter string, and the characters that are enclosed in the string values. The syntax is: 

```
%script 
SQLFORMAT DELIMITED delimiter left_enclosure right_enclosure 
```

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/deliminated.png)

For example:
```
%script 
SET SQLFORMAT DELIMITED ~del~ " " 
SELECT * FROM emp WHERE deptno = 20; 
```

Output: "EMPNO"~del~"ENAME"~del~"JOB"~del~"MGR"~del~"HIREDATE"~del~"SAL"~del~" COMM"~del~"DEPTNO" In this example, the delimiter string is ~del~ and string values such as EMPNO, ENAME, JOB and so on, are enclosed in double quotes.

## Sample Question:

Here is an example question around output formats:

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/sqlloader.png)

**Question:** To which output the above output is related?
**Answer:** SET SQLFORMAT LOADER

*Sourcing:*
*Content sourced from Oracle Machine Learning Documentation.*
*Example questions sourced from Udemy and other places.*


# Preparing For Oracle Machine Learning Using Autonomous Database 2021 Specialist Certification
### *A preparation guide*

*This certification is listed to expire August of 2022.  I assume this means they are launching a new test and possibly content for this course.*

## Introduction:

I have focused on Oracle certifications for the past two years. Some are easier than others. Two of the challenges of certifications are understanding where to find content and on which content to focus. Oracle does a great job of spelling out what you need to know. There have been a few instances where the study material did not match the exam well. To help others achieve this certification, here is a helpful guide. Based on experience, this guide should remain applicable for 1 to 2 years unless there is a dramatic change in content for the exam. What I am saying is that I have noticed Oracle tends to keep content and exams consistent between years.

I recommend the following sources for study preparation for this exam:
1.	<a href="https://education.oracle.com/">Oracle University</a>
2.	<a href="https://docs.oracle.com/en/database/oracle/machine-learning/index.html">Product documentation</a>
3.	<a href="https://www.udemy.com/">Udemy </a>
4.	<a href="https://apexapps.oracle.com/pls/apex/dbpm/r/livelabs/home">Oracle LiveLabs</a>
5.	<a href="https://blogs.oracle.com/machinelearning/">Oracle Machine Learning Blogs</a>

With any Oracle certification, you want to make sure that you balance your time between practicing test questions, reading the source material, and performing hands-on labs.

## Core Content:

There are eight core topic areas for the 2021 exam. Below is information on each topic to get you started.

2021 Topic Areas:
1.	Introduction to Oracle Machine Learning and Oracle Autonomous Cloud Platform
2.	Creating Workspaces and Projects in Oracle Machine Learning
3.	Creating SQL Scripts and Running SQL Commands in Oracle Machine Learning
4.	Auto ML
5.	Notebooks in Oracle Machine Learning
6.	Collaborating Using Templates in Oracle Machine Learning
7.	Working with Jobs in Oracle Machine Learning
8.	Administering Oracle Machine Learning

Topic 1: In this topic, you should understand Oracle Machine Learning features and algorithms. Also, understand what Oracle Machine Learning is.

Topic 2: In this topic, you should understand how to create a workspace, create projects, and how managing them.  This section will test your knowledge of how the administrator role works.  

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/get-started-project-and-workspaces1.html">Get Started with Project and Workspaces</a>

Topic 3: This topic covers SQL scripts.  You need to understand how to create and run SQL commands.  This topic also touches on connection groups and restrictions on SQL commands.  I recommend memorizing the different interpreters that are available.  You should be comfortable with writing simple scripts.

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/use-scratchpad.html">Use the Scratchpad</a>

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/edit-your-notebook.html">Edit Your Notebook</a>

Topic 4: This topic covers three areas of AutoML: general knowledge of AutoML, AutoML with OML4PY, and user interface.  It is helpful to know what the Oracle AutoML pipeline is and how the individual pieces of the pipeline work.

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-automl-ui/index.html">Oracle Machine Learning AutoML User Interface</a>

Topic 5: This topic covers Notebooks on Oracle Machine Learning. To grasp this section, you should understand Zeppelin notebook technology, including features and how to use it.  Specific content covered in this section includes output formats, forms, and notebook versioning.  Three forms that you should understand include Select Forms, Text Input Forms, and Check Box Forms.

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/get-started-notebooks-data-analysis-and-data-visualization1.html">Get Started with Notebooks for Data Analysis and Data Visualization</a>

Topic 6: This section tests knowledge of templates and creating notebooks from templates.

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/use-library-collaborate-users.html#GUID-09AD4419-B0DE-4F3B-9FEB-0ABA3AFD6E7A">Use Example Templates</a>

Topic 7: This topic will test your knowledge of Oracle jobs.  You need to know what Oracle Jobs is, how to schedule Jobs, and view Job logs.
See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/get-started-jobs.html#GUID-27D680E4-5F9A-42DC-BE37-01DC450D2CC5">Get Started with Jobs</a>

Topic 8: This topic area tests knowledge on the administrator role and managing users.  Understand what an administrator can do versus a developer.  Learn how to manage users and user resources.

See <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/omlug/administer-oracle-machine-learning.html#GUID-E74F0E2E-EEE5-4421-A0BB-96A58811C04A">Administering Oracle Machine Learning</a>

## Sample Test Questions:

Topic 1: Which Oracle Cloud Services are compatible with Oracle Machine Learning?
*Answer: Autonomous Transaction Processing, Autonomous Data Warehouse Cloud Service, and Autonomous Analytics Cloud*

Topic 2: Which components are contained in a workspace?
*Answer: Notebooks and Projects*

Topic 2: Which workspace permissions are available in Oracle Machine Learning?
*Answer: Viewer, Manager, and Developer*

Topic 3:  In which file format can SQL scripts can be saved in Oracle Machine Learning?
*Answer: JSON*

Topic 3:  Which SQL statement is available in Autonomous Data Warehouse?
*Answer: None of These: ALTER PROFILE, ALTER TABLESPACE, CREATE TABLESPACE*

Topic 4: Which statements pertaining to Algorithm Selection are true?
*Answer: oml.automl.AlgorithmSelection supports classification and regression algorithms ,no single model works best for all problems, we specify the dataset and the number of algorithms to evaluate*

Topic 5: Which output formats are supported by the SET SQLFORMAT command?
*Answer: JSON, CSV, HTML*

Topic 5: Which output format supported by the SET SQLFORMAT command produces pipe-delimited output?
*Answer: LOADER*

Topic 6: What are the different templates available in Oracle Machine Learning?
*Answer: personal templates, shared templates, and example templates*

Topic 7: When scheduling a job, which notebooks are available for selection?
*Answer: notebooks owned by the user, notebooks shared by other users*

Topic 8: Which role can access the Compute Resources page?
*Answer: Administrator*

*Source: All sample test questions pulled from the 2021 Oracle University certification coursework.*

Udemy provides additional sample test questions for this certification that you can buy. Click <a href="https://www.udemy.com/course/1z0-1096-21-oml-using-autonomous-database-2021-specialist/">here</a> to be directed to the 2021 sample test questions.

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/image1.png)
image: Udemy Prep Tests

# Source Material:

Oracle documentation is maintained a <a href="https://docs.oracle.com/en/database/oracle/machine-learning/oml-notebooks/">docs.oracle.com</a>. You should spend a large amount of your time going through this documentation.  In my experience, test questions come from information in the documentation.  

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/image2.png)
image: Oracle Machine Learning Documentation Landing Page

# Hands-On Experience:

Hands-on experience is an important part of the study process.   Oracle provides free hands-on experience options through LiveLabs.  

Here is a list of LiveLabs course that can help you prepare for this exam:
* Introduction to Machine Learning Algorithms on ADB
* Machine Learning on ADB - Choose your journey
*	Introduction to Oracle Machine Learning Notebooks
*	Detect anomalies with OML4SQL using one-class support vector machine (SVM)
*	OML4Py
*	Get started with Oracle Machine Learning Fundamentals on Oracle Autonomous Database
*	Introduction to Machine Learning Algorithms on ADB
* Predicting Auto Claim Fraud with Oracle Machine Learning
*	Introduction to Oracle Machine Learning for Python on Autonomous Database
*	Learn Analytics and Machine Learning with SailGP
*	Machine Learning on Autonomous Database

There is much more you can choose from than what I list here.

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/image3.png)
image: Oracle LiveLabs

## Oracle’s Recommended Test Prep:

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/image4.png)
image: Exam Topics 1-3

![image](https://github.com/nicktoscano/oml_cert_2021/blob/main/images/image5.png)
image: Exam Topics 4-5

## Good Luck on your exam!

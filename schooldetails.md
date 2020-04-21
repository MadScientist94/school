Following are the components used in these application,  along with injected service and used routing

1. Login page component
1. School page component 
1. school details page
1. Department page component 
1. department details page
1. Student page component 
1. student details page 
1. modal component for student entry-form
1. Subject page components
1. Marks page component
1. Teachers page components  
1. teachers details  page 
1. teachers modal component
	

### Login page:
Page  contain login form and create login form
### Login Form: 
*	Contains: input=> user name and password
*	if wrong password entered alert message pops 
*	if right password entered the this page should routed to school component 

|Form Element	|Data stored in serve|
|---------------|-|
|User name	    ||
|password	    ||

### Create user form:
* 	**contains**: input's => name, email, phone number , city, pincode, password,confirm password, save button, reset button, close button
* 	validation confirm password and password should be same

|Form Element	|Data stored in serve|
|-|-|
|Name 	|Name |
|Mail	|Mail|
|Phone	|Phone|
|City	|City|
|Pincode	|Pincode|
|Password	|Password|
|Confirm password| |
|	|userId|



### Main page component:
this page contains a child router and navigation bar with link buttons (school, department, student, subject, mark, teacher, logout.

### Schools component:
* 	table to display school list  with pagination.
* 	Create school modal: input=> school name, address, pincode, mail Id, phone number,register year, save button , close button

|Form Element|	Data stored in serve|
|-|-|
|School name	|School name|
|Address	|Address|
|Pincode	|Pincode|
|Mail	|Mail|
|Phone	|Phone|
|Registered year	|Reg year|
|	|School id|
	

### Department component:
* 	Contain: table to display department list 
* 	Form : input=> department  name, school name with id

|Form Element	|Data stored in serve|
|-|-|
|department name|department name|
|School name	|School id|
|	|Department id|


Student component:
* 	Contain : table to display students list with pagination
* 	Student modalComponents: input=> first name, second name school name, department name, date of birth , gender

|Form Element	|Data stored in serve| 
|-|-|
|First name	|First name|
|Second name	|Second name|
|Department name	|Department id|
|Date of birth	|Date of birth|
|Gender	|Gender|
|	|Student id|

### Subject component:
* 	Contains :table with subject list
* 	Subject modal: input=>subject name

|Form Element	|Data stored in serve|
|-|-|
|Subject name	|Subject name|
| |		Subject id |

### Mark component:
* 	Contains: table displaying mark list
* 	Form: input=>  student name subject name  marks

|Form Element	|Data stored in serve|
|-|-|
|Student name	|Student id|
|Subject name	|Subject id|
|mark	|Mark|

### Teacher component:
* 	Contains : table  display teacher list
* 	Form: input=> teachers name and  gender

|Form Element	|Data stored in serve|
|-|-|
|Teacher name	|Teacher name|
|Gender	|Gender id (array set in main component)|
|	|Teacher id|

### School page:
As the picture displays, page contain filter box on key up the page should filter the list according to the text in the text box. Followed by table filled with school list. And the list displays school-list according to no of list school should displayed and which page is active in the pagination. On double click in the name will route the page to student details page

### In the following figures
* 	Yellow button denotes edit button. 
* 	Red button denotes the delete button.
* 	Blue/green button above the table represent the create new school 

###  School, department, student, teacher components share the same format	 

![images](./img/school_table.png)
#####  figure :School Table
![images](./img/department_table.png)
##### figure : Depaetment Table
![images](./img/student_table.png)
##### figure :Student Table
![images](./img/teacher_table.png)
##### figure :  Teacher Table

![images](./img/createschoolForm.png)
##### figure : create school form

![images](./img/createDepartmentForm.png)
##### figure : create department form
![images](./img/updateDepartmentForm.png)
##### figure : update department form

![images](./img/createTeacherForm.png)
##### figure : create teacher form
![images](./img/updateTeachersForm.png)
##### figure : update teacher form

![images](./img/createStudentForm.png)
##### figure : create student form
![images](./img/updateStudentForm.png)
##### figure : update student form


### School details  page and its update function

![images](./img/schoolDetailsPage.png)
##### figure : school details page
![images](./img/editSchoolDetailsPage.png)
##### figure : edit function on student details page
On clicking update function static form element should be convert to input elements and show update and the close button

![images](./img/departmentDetailsPage.png)
##### figure : department details page
These page  should show number of students in the department  on edit the no of student should be hidden
![images](./img/editDepartmentDetailsPage.png)
##### figure : edit function on department details page

### Subject table
![images](./img/subjectTable.png)
##### figure : subject table
![images](./img/createSubjectForm.png)
##### figure : create subject form
![images](./img/updateSubject.png)
##### figure : update subject form


![images](./img/markTable.png)
##### figure : mark table
![images](./img/createMarkForm.png)
##### figure : create mark form
On double tap on the mark to edit the mark: on enter or click tick button update the value
![images](./img/updateInMarkForm.png)
##### figure : update mark form
On double tap on the mark to edit the mark: on enter or click tick button update the value


### Student detail page
![images](./img/studentDeatilspage.png)
##### figure : student details page
In student list when we click students page the page routed to student details page. 
Student details page contain students entry form and mark table; all the data should be filtered according to the concern student id and the mark table should have default student id.
![images](./img/cardInStudentDetailsPage.png)
##### figure :  using a card from BS4 we display some info about the students

Next to the mark table the card shows their gender and the level of mark the obtained mark
Mark component should not display the student name in the display
![images](./img/editStudentDetailsPage.png)
##### figure : edit function in the student details page

On editing the page display the edit option of the  student form
![images](./img/homeWorkInStudentDetailsPageWhole.png)
##### figure : home work list in student details page

On clicking home work the page displays the home work allotted to the concern person
Description, start time, end time, and stuatus are editable while double click over them it should change to editable format
On clicking teacher name in the teacher list it should navigate to teachers details and also to create the home work and display the list below the teacher list


![images](./img/teacherDetails.png)
##### figure : teachers details page with home work list assigned by the teacher
![images](./img/createHomeWorkForm.png)
##### figure : create home work 
![images](./img/updateHomeWorkForm.png)
##### figure : update home work
    

    
 


 

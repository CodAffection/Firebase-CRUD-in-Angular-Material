# Firebase CRUD in Angular Material

###### Before Running this Project
 1. Install npm packages using 'npm install' command.
  
Content discussed : 
 - firebase crud operations
- angular form submission
- render dynamic dropdown
- create popup notification in angular material

## Issues and Fixes
**hireDate not inserted to firebase** <br/>
**reason**: forgot to formate the date before insert/ update operation. <br/>
**fix** :  <br/>
add DatePipe to app.module.ts providers array - [updated line](https://github.com/CodAffection/Firebase-CRUD-in-Angular-Material/blob/c161712fb952baba9cb189ce70c9f1a8ecf096fc/Firebase%20CRUD%20with%20Angular%20Material/src/app/app.module.ts#L31) <br/>
update in employeeService.ts <br/>
inject the DatePipe to constructor- constructor(...,private datePipe: DatePipe){} [updated line](https://github.com/CodAffection/Firebase-CRUD-in-Angular-Material/blob/1198716b50ffcc2b141ddffbcb165c8434b26197/Firebase%20CRUD%20with%20Angular%20Material/src/app/shared/employee.service.ts#L11) <br/>
update functions : insertEmployee & updateEmployee for hireDate formatting <br/>
hireDate: this.datePipe.transform(employee.hireDate, 'yyyy-MM-dd') [updated line](https://github.com/CodAffection/Firebase-CRUD-in-Angular-Material/blob/e5b0cc739b41b3680dbc1f6fc8f03beda53ca993/Firebase%20CRUD%20with%20Angular%20Material/src/app/shared/employee.service.ts#L55)<br/>

 
 # Step By Step Explanation
 
 Video Tutorial : https://youtu.be/hfhlzY3U27M
 
 <a href="http://www.youtube.com/watch?feature=player_embedded&v=hfhlzY3U27M
" target="_blank"><img src="http://img.youtube.com/vi/hfhlzY3U27M/0.jpg" 
alt="Video Tutorial for Firebase CRUD in Angular Material" width="500" height="400" border="10" /></a>

# Complete Angular Material Tutorial
1. https://goo.gl/XmR6Li - Form Design.  
2. https://goo.gl/3VQn29 - Firebase CRUD.[this one ]
3. https://goo.gl/5h59y5 - Angular Material Data Table.



# All Video Tutorial Series
| Series        | Video PlayList          |
| ------------- |:-------------:|
| Angular 7|https://goo.gl/vN9LFd  |
| Asp.Net MVC|https://goo.gl/gvjUJ7  |
| Asp.Net Core|https://goo.gl/scJc4f  |
| Node JS|https://goo.gl/viJcFs  |
| Web API|https://goo.gl/itVayJ  |
| Angular Material|https://goo.gl/TbDQnT  |
| MEAN Stack|https://goo.gl/YJPPAH  |
| C# Tutorial|https://goo.gl/s1zJxo  |
| Asp.Net WebForm|https://goo.gl/GXC2aJ  |
| Angular 5|https://goo.gl/ahk39S  |
| Angular 4|https://goo.gl/Ha71kq  |
| C# WinForm|https://goo.gl/vHS9Hd  |
| MS SQL|https://goo.gl/MLYS9e  |
| Crystal Report|https://goo.gl/5Vou7t  |
| CG Exercises in C Program|https://goo.gl/qEWJCs  |

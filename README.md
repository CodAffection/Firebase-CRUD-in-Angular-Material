# Firebase CRUD in Angular Material
  
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

## Get the Code

```
$ git clone https://github.com/CodAffection/Firebase-CRUD-in-Angular-Material.git
$ cd CodAffection/Firebase-CRUD-in-Angular-Material/Firebase CRUD with Angular Material
$ npm install
//run the app
$ ng serve
```

 ## How it works ?

 :tv: Video tutorial on this same topic  
 Url : https://youtu.be/hfhlzY3U27M
 
<a href="http://www.youtube.com/watch?feature=player_embedded&v=hfhlzY3U27M
" target="_blank"><img src="http://img.youtube.com/vi/hfhlzY3U27M/0.jpg" 
alt="Video Tutorial for Firebase CRUD in Angular Material" width="500" height="400" border="10" /></a>


## Complete Angular Material Tutorial
1. Form Design - https://goo.gl/XmR6Li 
2. Firebase CRUD - https://goo.gl/3VQn29 [_this one_]  
3. Angular Material Data Table - https://goo.gl/5h59y5
4. Material Popup - https://goo.gl/NNf5sp
5. Material Confirm Dialog - https://goo.gl/pr8rs6


| :bar_chart:               |  List of Tutorials   |   | :moneybag:           | Support Us                           |
|--------------------------:|:---------------------|---|---------------------:|:-------------------------------------|
| Angular                   |http://bit.ly/2KQN9xF |   |Paypal                | https://goo.gl/bPcyXW                |
| Asp.Net Core              |http://bit.ly/30fPDMg |   |Amazon   Affiliate    | https://geni.us/JDzpE                |
| React                     |http://bit.ly/325temF |   |
| Python                    |http://bit.ly/2ws4utg |   | :point_right:        | Follow Us                            |
| Node.js                   |https://goo.gl/viJcFs |   |Website               |http://www.codaffection.com          |
| Asp.Net MVC               |https://goo.gl/gvjUJ7 |   |YouTube               |https://www.youtube.com/codaffection  |
| Flutter                   |https://bit.ly/3ggmmJz|   |Facebook              |https://www.facebook.com/codaffection |
| Web API                   |https://goo.gl/itVayJ |   |Twitter               |https://twitter.com/CodAffection      |
| MEAN Stack                |https://goo.gl/YJPPAH |   |
| C# Tutorial               |https://goo.gl/s1zJxo |   |
| Asp.Net WebForm           |https://goo.gl/GXC2aJ |   |
| C# WinForm                |https://goo.gl/vHS9Hd |   |
| MS SQL                    |https://goo.gl/MLYS9e |   |
| Crystal Report            |https://goo.gl/5Vou7t |   |
| CG Exercises in C Program |https://goo.gl/qEWJCs |   |

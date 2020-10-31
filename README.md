# yashryTask
the problem:
program that can price a cart of products, accept multiple products, combine offers, and display a total detailed bill in different currencies 

the solution:
i wrote a program that enable the user to select the currency s/he wants and inputs the quantity s/he wants then get the bill wich contains the subtotal , taxses, available discounts,and the total price after adding the taxes and subtracting the total amount of discount based on the selected currency.
 
 
Running Application:
1-open the "onlineshopping.sql" file and run the script to create the database
2-open the Cred.php file and change the database configuration accoarding to yours
3-Open the Command Prompt
4-Change the Directory to the Project's Path
5-write the following Command line 
	php -S localhost:1234/index.php (or any available port)
6-Open the link and start your trial   


-description of the exist files:
1- Controllers Folder: contains "ProductContr.php" file implements all the functionalities except the dealing with database this for model.
2- Model folder: contains "Product.php" this represent the Product Entity in database , and "productDao.php"  this class that deal with the database concept of Data Access Object.
3- Views folder : contains -"index.tpl" this is the home page where the user enters the input. 
                           -"bill.tpl" this page shows the output based on the users input.
                           -"route.php" this file handles the page routings accoarding to the Get request it calls the functions from the controller and pass the required data                               to the next page
4-lib folder : this is Smarty library which used to separate the front end and the back end
5-public folder : this contains Css Folder wich contains the css files for styling.
6- Cred.php: this file contains the defines variables through the project such as DbName , Servername ...etc.
7-db.php file : implements the database configuration and connection using (Signlton Design Pattern).
8-onlineshopping.sql : this contains the script of the used database through the project.
9-index.php file which is the start point of the project

-the solution is full stack but it focused more on the back-end may be if i had more time i would make the ui more creative but i used to deliver the task in the estimated time:)

-reasons behind technical choices 
 -used Smarty Template Engin to separate the back-end and front-end to not get confused while reading or maintaining the code.
 
 -used OOP MVC design patten for faster development process whichalso  makes the project more readable easy to maintain and separate each parts
      -MODEL: used for describe the entities in database.
      -CONTROLLER: witch handles the functionalities and also acts as a link between a user and the system.
      -VIEW: for UI This level creates an interface to show the actual output to the user. 
    and also makes The Modification doesn't affect the entire Model.
    
 -used Singlton Design Pattern while creating the database to avoide multiple connections .
 
 
 -trade off i might made if i had more time 
  -i would improve the user interface to be more easy to use i would make a logging in and error handling 
  -i would learn how to use REST API this is missed in the project ..i dealt as normal webpages actually i asked if its availabe to use it but i didnt get answer!
  -i would use Sqlite instead of mySql which is much better for small tasks 
  
  
  

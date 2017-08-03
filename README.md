# stock-management
Stock Management System open source project with procedural php, MySQL, bootstrap, and jquery. This application is based on web application and develop with procedural php, MySQL database, jquery, datatables plugins, and bootstrap. This application provides the users to manage brands, category, product, orders, and report.

In brands page, the admin can add, update, and remove the brand’s information. In product section, the admin can add the product information and manage the stock. In order section, the application will manage the stock of the product and generates the total amount of payment to be pay by the client. The application can also generate the orders report on based on the month you select.

Requirements
PHP Version +5.4.4
Web Server ( Recommended : Apache with PHP and Mysqli )
Features
View of a total number of brands, categories, product, and orders.
Add, update, and remove brands information.
Add, update, and remove categories information.
Add, update, and remove product details.
Add, update, and remove orders details.
Print orders invoice.
Update orders payment.
Generate the orders report by selecting specific start and end date.
Change Password
Change Username
Users
Admin
Username: admin
password: password
Change the VAT
To change the vat number, all you have to do is go to the order.js file which is located at [custom/js/order.js] and search for subAmount function. In the line of 555, you will see the VATvariable, change the VAT number that you desired. To change the vat number in the front end of the application, go to orders.php and at the line of 369, you will see the VAT label, change it the number you desire.

Download Online Stock Management System
Please Read:

While creating the database for this system, either you can create the name of the database as a stock or change the name at the php_action/db_connect.php file. As shown below:

?
db_connect.php

<php 
$localhost = "127.0.0.1"; 
$username = "root"; 
$password = ""; 
$dbname = "stock"; 
 
// db connection 
$connect = new mysqli($localhost, $username, $password, $dbname);
 
// check connection 
if($connect->connect_error) {
  die("Connection Failed : " . $connect->connect_error);
} else {
  // echo "Successfully connected";
}
 
?>

# CISC3003-Team08-FinalProject
 Github Repo:<https://github.com/HUIGUANHAO/CISC3003-Team08-FinalProject>


Hello, we are Team08: Pair02&03&23
Our team number:
>* DC126711 HUI GUANHAO
>* DC027495 DENG YIFAN
>* DC127910 CUI JIANFU
>* DC126057 HE GUO JHON KOU JING
>* DC125611 WONG KUOK LEONG
>* DC127947 MA YINGCHEN


Our team project is aiming to build a Macau House Rental Platform, an innovative digital solution designed to simplify the property rental process in Macau.  The platform bridges communication between landlords and tenants by providing a range of services to landlords and tenants, simplifying the transaction process. We specialize in developing rental management platforms that allow users to seamlessly manage rental activities through a web interface.  Our platform supports a variety of features, including user authentication, property listings, and account management.  Users can log in or register, view rental listings, adjust filters, and manage their profiles.   
  >We will use the following tools and languages to assist in the development:
  >- HTML
  >- CSS
  >- Javascript
  >- jQuery
  >- PHP
  >- MySQL


# Database Deployment
The first step is to start our server, which requires us to install XAMPP or WAMP and MySQL already on our computer.
>1. We start the XAMPP or WAMP server first
>2. Let's open the Admin screen
>3. Select import
>4. we import the rentsys.sql file, which will create the required database and tables:

![alt text](<My screen shots/database_setup.png>)

After that we set the password of the user in conn.php file so that we can complete the connection to the database

```php
<?php
//connect to the database
    $conn = mysqli_connect("localhost", "root", "root", "rentsys");
    if(!$conn){
        die("Failed to connect to the database server");
    }
    //Setting character set
    mysqli_query($conn, "set name utf8");
?>
```

Now we can successfully link to the database!


# Main function
We will implement some of the features including but not limited to the following:

>1. Tenant/landlord Login/Sign up
>2. Rental listing browsing
>3. Housing information screening
>4. User profile management
>5. Order management
>6. House information management(landlord)

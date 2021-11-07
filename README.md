# Pierre's Sweet and Savory Treats 2.0 

#### By Dylan Allison-Damitz

## Technologies Used :floppy_disk:
* _NuGet Package Manager_
* _C#_
* _.Net 5_
* _REPL_
* _MySQL_
* _MySQL Workbench_
* _Microsoft Enity Framework_

## Description :page_with_curl:
_A C# application using many-to-many relationships and authentication functionality, this website allows Pierre's customers to log in and sign out of their personalized accounts. Only customers with accounts can access create, update, and delete functionality. This project uses the Microsoft Entity Framework and migrations to create and store database inputs automatically_

## Setup/Installation Requirements :triangular_ruler:

* Clone github repo: https://github.com/Dylan-Allison-Damitz/Pierres_Bakery2.0.git
* Navigate into the directory from your desktop: `cd Pierres_Bakery2.0`
* Open in Vs code: `code .`
* Navigate to the Factory directory using the terminal: `cd Bakery`
* To install dependencies, run: `dotnet restore`


## Updating appsettings.json

* In order for the Entity Framework to automatically create the database, you'll need to have your `appsettings.json` set up properly 
* Create an `appsettings.json` file within the `Bakery` folder
* Copy and paste the following code into the file:

```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=dylan_allison_damitz;uid={YOUR-USERNAME};pwd={YOUR-PASSWORD};"
  }
}
```
* Make sure you remove the curly brackets after entering in your username and password
* Once your database connection is complete, return to the terminal and run `dotnet build` to compile the project

## Implementing Migrations

* Once `appsettings.json` has been created and filled out, assure you are still within the `Bakery` folder and enter the command `dotnet tool install --global dotnet-ef --version 3.0.0` to ensure Enitity Framework is installed on your system
* Type `dotnet ef database update` to assure any changes have been accounted for
* `dotnet run` will compile the project and launch in your local browser

## License :clipboard:
MIT &copy; 2021 _Dylan Allison-Damitz_
## Contact Information :mailbox:

_Dylan Allison-Damitz:
dylandamitz@gmail.com_

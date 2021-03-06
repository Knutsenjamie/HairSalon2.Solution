# _Claires Salon_

### _C# Database Basics_

##### By:
#####  _**Jamie Knutsen**_ _©2021_


## Technologies Used

* _Visual Studio Code_
* _.NET_
* _C#_
* _Entity Framework Core (EF Core)_
* _ASP.NET Core MVC_
* _MySQL_
* _MySQL Workbench_


## Description: 
This project was designed to practice building basic web applications with C# using mysql databases and the MVC model.


## Setup/Installation Requirements
_You can view this webpage by checking out the url:_
https://github.com/Knutsenjamie/HairSalon2.Solution

### Prerequisites
* [C# & .NET] Install at (https://dotnet.microsoft.com/download/dotnet/thank-you/sdk-5.0.100-macos-x64-installer) (If Mac) OR https://dotnet.microsoft.com/download/dotnet/thank-you/sdk-5.0.102-windows-x64-installer (If Windows)
* [dotnet script] After installing C# and .NET, run the command 'dotnet tool install -g dotnet-script' in your computer's terminal or text editors terminal. 
* A text editor such as [VS Code] (https://code.visualstudio.com/)
* For the database, you'll need to install MySQL (https://dev.mysql.com/downloads/file/?id=484914). I also suggest using MySQL workbench as a GUI for viewing and importing databases. 

### Installation
1. Open terminal
2. Input these commands into terminal's command line 'cd desktop'
3. Clone https://github.com/Knutsenjamie/HairSalon2.Solution from github
4. Open MySQL Workbench, and use the Navigator tab to go to the 'Administration' window. 
    * Then, go to 'Import Options', and then select 'Import from Self-Contained File'.
    * Grab the jamie_knutsen.sql file from https://github.com/Knutsenjamie/HairSalon2.Solution repository
    * Navigate to 'Default Schema To Be Imported To', then select 'New'
    * Enter in jamie_knutsen for the database name. Then, click 'Ok'
    * Click 'Start Import'
    * Go back to the Navigtor tab and go to 'Schemas'
    * Click 'Refresh All'. The imported database should now appear. 
4. Run the command 'code .' in your computer's terminal
5. Open VS Code or other preffered text editor terminal within the project file
6. To install and make sure all needed packages are up-to-date, navigate into the HairSalon folder from root directory by entering 'cd HairSalon' in terminal.
    * Type the command 'dotnet restore' to update and restore all needed packages and dependencies to run application.
7. In order to use the database, run the command 'touch appsettings.json' in the HairSalon directory of the project. 
    * The, enter in your own approppriate username (or enter 'root' in the YOUR-USERNAME-HERE field), and whichever password you used to open, use, and create the imported database in MySQL Workbench- use it and enter it as follows in this line 'database=jamie_knutsen;uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE]' *do NOT actually put []- this is just for visual purposes to see where to change the information*
    * Finally, copy it like in this example, 
    '{
    "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=jamie_knutsen;uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE];"
    }
    } 
    and paste it into the appsettings.json to use the database. *WARNING: This file should automatically be ignored AS LONG AS it is in the HairSalon directory and NOT the root directory (as it is listed in the .gitignore). However, Be aware of what you are committing and pushing to avoid pushing your personal username and password- as it is sensitive data* Your database should now be connected. 
8. Navigate into root directory folder in terminal 'cd HairSalon2.Solution' and  enter command 'dotnet run' or 'dotnet watch run' to run the program. 

## Licensing

Licensed under the [MIT License](license).

## Contact Information

_Jamie Knutsen (knutsenjamie@yahoo.com)_

## Schema 

<!-- ![Schema Image](files/Users/thatbejamie/Desktop/jamiesschema.png) -->
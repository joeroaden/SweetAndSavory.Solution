# _SweetAndSavory_

#### By _Joe Roaden_

#### _An MVC application using Databases and MySQLWorkbench used to track flavors and sweets using a many to many relationship_

---
## Table of Contents
[Technologies Used](#technologies-used)  
[Description](#description)  
[Setup/Installation Requirements](#setup-and-installation-requirements)  
[Known Bugs](#known-bugs)  
[License](#License)

---
## Technologies Used

* _C#_
* _.NET_
* _HTML_
* _CSS_
* _SQL Workbench_
* _Entity Framework_
* _MVC_
* _Identity Framework_

---
## Description

_An MVC application using Databases and MySQLWorkbench used to track flovors and sweets using a many to many relationship.  This project has user authentication and new users can create an account to add, edit or delete flavors and treats.  Anonymous users can view existing flavors and their respective treats, but only authorized users can make updates_

---
## Setup and Installation Requirements

<details>
<summary><strong>Initial Setup</strong></summary>  

1. Copy the git repository url: https://github.com/joeroaden/SweetAndSavory.Solution 
2. Open a shell program and navigate to your desktop.
3. Clone the repository for this project using the `git clone` command and including the copied URL.
4. While still in the shell program, navigate to the root directory of the newly created file named `SweetAndSavory.Solution`.
5. From the root directory, navigate to the `SweetAndSavory` directory.
6. Move onto SQL Workbench instructions below to re-create database necessary to run this project.
</details>

<details>
<summary><strong>SQL Workbench Configuration</strong></summary>

1. Create an `appsetting.json` file in the `SweetAndSavory` directory of the project  
   <pre>SweetAndSavory.Solution
   └── SweetAndSavory
    └── <strong>appsetting.json</strong></pre>
2. Insert the following code [^1]  
    ```json
    {
      "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=joe_roaden;uid=root;pwd=[YOUR-PASSWORD-HERE];"
      }
    }
    ```

3. Once `appsettings.json` file has been created, navigate back to SQL Workbench.
</details>

<details>
<summary><strong>To Run</strong></summary>

1. Navigate to:  
   <pre>SweetAndSavory.Solution
   └── <strong>SweetAndSavory</strong></pre>

2. Run `$ dotnet restore` in the console.  
3. Run `$ dotnet database update` in the console.  
4. Run `$ dotnet run` in the console
</details><br>

This program was built using *`Microsoft .NET SDK 5.0.401`*, and may not be compatible with other versions. Your milage may vary.

---
## Known Bugs

* Any known bugs

---
## License

_See MIT License Attached_

[Copyright](/LICENSE) © 2022 Joe Roaden

---
### Footnotes

[^1]: You must include your password in the code block section labeled `[YOUR-PASSWORD-HERE]`.
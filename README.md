# ExecuteAutomationWebApp
This application is used for automating selenium and coded UI frameworks course

#Automation framework development with Selenium C sharp
https://www.udemy.com/framework-development-with-selenium-csharp-advanced

#Advanced framework development with Coded UI Test 2015
https://www.udemy.com/framework-development-with-cuit

#How to Compile application ?
All you have to do is 

1. Clone the repo or download it
2. Open the project in Visual studio 2013/2015
3. Just build the project and run in any browser of your interest, the application will launch and ready for automation

# Advanced Topic
##What will happen while building project
The project will automatically create database for you in the default database server, since the connection string in Web.config is given as This
```xml
  <connectionStrings>
    <add name="EmployeeDb" connectionString="Data Source=.;initial catalog=EmployeeDB;integrated security=True" providerName="System.Data.SqlClient" />
  </connectionStrings>
```

## Troubleshooting
If the database does not restore for some reasons, then run the database script located in DatabaseScript folder of the repo in SQL Server management studio

## ExecuteAutomation Employee App running on public Server
We have deployed ExecuteAutomation Employee App running in public server and it can be accessed from here http://eaapp.somee.com/

### Connection string details

```xml
workstation id=EAEmployeeDB.mssql.somee.com;packet size=4096;user id=kartmcad_SQLLogin_1;pwd=wtzaxoan1l;data source=EAEmployeeDB.mssql.somee.com;persist security info=False;initial catalog=EAEmployeeDB
```

## More articles
For more articles visit http://www.executeautomation.com

#### customisations required to get this to work with visual studio 2019 community edition
1) Execute the following in the Package Manager Console to work around the roslyn error:
Update-Package Microsoft.CodeDom.Providers.DotNetCompilerPlatform -r

2) Change database connection string in web config
 -> Integrated Security=True to user=sa;password=P@ssw0rd1;

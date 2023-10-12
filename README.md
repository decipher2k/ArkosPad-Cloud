# ArkosPad Cloud
<br>
Setup hosting:<br>
1.) Setup IIS or dotNet linux with Apache hosting on your server<br>
2.) Install MySQL<br>

Backend (dotNet):<br>
4.) Setup an app in IIS with the endpoint /api or setup dotnet hosting with Kestrel and create a reverse proxy to the /app subdirectory of your wwwroot.<br>
5.) Copy contents of the file "ArkosPad Cloud - Backend.zip" to the root directory of the dotnet app.<br>
6.) Edit user.conf and enter the password for the "admin" user.<br>
7.) Edit dbsettings.conf and enter the MySQL connection string. The MySQL user has got to have the rights to create tables.<br>
8.) run https://-hostname-/api/Install/Install to initialize the database and setup the admin user.<br>
<br>
Frontend(Node.js):<br>
9.)  Copy contents of the file "ArkosPad Cloud - Fronted.zip" to your wwwroot.<br>
10.) Create rewrite rules for the Angular app.<br>
11.) Edit ./assets/config.json to match your hostname.

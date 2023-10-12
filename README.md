# ArkosPad Cloud
<br>
<b>Setup hosting:</b><br>
1.) Setup IIS or dotNet linux with Apache hosting on your server<br>
2.) Install MySQL<br>
<br>
<b>Backend (dotNet):</b><br>
1.) Setup an app in IIS with the endpoint /api or setup dotnet hosting with Kestrel and create a reverse proxy to the /app subdirectory of your wwwroot.<br>
2.) Copy the content of the file "ArkosPad Cloud - Backend.zip" to the root directory of the dotnet app.<br>
3.) Edit user.conf and enter the password for the "admin" user.<br>
4.) Edit db.settings.conf and enter the MySQL connection string. The MySQL user has got to have the rights to create tables.<br>
5.) Run https://-hostname-/api/Install/Install to initialize the database and setup the admin user.<br>
<br>
<b>Frontend (Node.js):</b>b><br>
1.) Copy the content of the file "ArkosPad Cloud - Fronted.zip" to your wwwroot.<br>
2.) Create rewrite rules for the Angular app.<br>
3.) Edit ./assets/config.json to match your hostname.
<br><br>
<b>Caveats:</b><br>
-Currently only single user mode ("admin"), until the usermanagement has been repaired.

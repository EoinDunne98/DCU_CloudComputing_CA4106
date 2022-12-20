In order the run the *"manage.py"* , you **MUST** be within a python virtual environemt.

You must also be running a Google Proxy that connects to the SQL Instance. Do this by running the following command in a Google SDK Console. (Note that you **MUST** be on an authorised login)

**cloud_sql_proxy.exe -instances="cloud-computing-project-272315:europe-west1:computing-project"=tcp:3307**

Once the proxy is listening for connections on Port 3307 you must now navigate to the file that contains *"manage.py"* within the command prompt. Now enter the following command,

**env\scripts\activate**

Once you are within the virtual environment, you can then run 

**python manage.py runserver**

This is for local testing only. The deployed website can be seen on

**https://cloud-computing-project-272315.appspot.com/**

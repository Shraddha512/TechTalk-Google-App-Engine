<h1>Developing Applications to be deployed on Google App Engine</h1>

These Steps are for developing Apps in Python on Linux machines. For other languages and platforms, [visit here for installation steps](https://cloud.google.com/appengine/downloads?hl=en_US&&&&&&_ga=1.220381914.352912814.1446512540#Google_App_Engine_SDK_for_Python)

<h3>Download SDK </h3>
Download Google App Engine SDK (For Python) [here](https://cloud.google.com/appengine/downloads?hl=en_US&&_ga=1.153233146.352912814.1446512540#Google_App_Engine_SDK_for_Python).

<h3>Installation of SDK on Linux </h3>

The downloaded SDK is in .zip format. To install the SDK, perform the following steps:

* If needed, install the unzip utility package:
~~~
sudo apt-get install unzip
~~~

* Navigate to the location where the SDK was downloaded. Extract the contents by:
~~~
unzip google_appengine_<your version number>.zip 
~~~

* Add the google_appengine directory to your PATH:
~~~
export PATH=$PATH:<insert path to the folder>/google_appengine/
~~~

* Make sure Python 2.7 is installed on your machine using the following command:
~~~
/usr/bin/env python -V
~~~

  The output should look like this: Python 2.7.<number>. If Python 2.7 isn't installed, install it now using the 
installation instructions for your Linux distribution by following the instructions mentioned [here](https://docs.python.org/2/using/unix.html#getting-and-installing-the-latest-version-of-python)

<h3> Deploying your App on the Google App Engine </h3>

* Once you are ready to deploy your application on Google App Engine, proceed [here](https://console.developers.google.com/start/appengine?_ga=1.210813527.352912814.1446512540&pli=1)
  to create a New Project. 
* Provide a Project name and a Project ID will be automatically generated for you. If you need to supply a custom 
  Project ID, click on Edit to supply one.
 ~~~
 NOTE: The project ID associated with the project is permanent and cannot be changed once a
        project is created. Please save the project ID for future use.
 ~~~
 
* Click on Create to create the Project.
 
* Once the project is created, perform the following steps in your local directory to deploy your app:
 ~~~
 <path to google_app_engine>/google_appengine/appcfg.py -A <your Project ID> update <path to the folder containing app code>/guestbook/
~~~

* To access more information about the Project, access the Project Dashboard here. A Sample Project Dashboard looks like this:
![dashboard](https://cloud.githubusercontent.com/assets/9305577/10953963/e4cce1ee-8318-11e5-874b-c6b300620e57.png)

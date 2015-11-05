<h1> Guestbook Application written in Python </h1>

  This application has been created by following the instructions on the [Google App Engine Tutorial Page](https://cloud.google.com/appengine/docs/python/gettingstartedpython27/introduction) 
</h3>

<h3> Purpose of the App </h3>

The app is a Simple GuestBook Application that explores some of the features of Google App Engine. Different users, 
either logged in or anonymous, can sign different guestbooks and these are visible for all to see with the latest entry
being the first one visible on the screen.

<h3> Working </h3>
* Users are authenticated via Google's inbuilt authentication system by making use of the authentication system used for 
Google's E-mail Service,GMail.
* The guestbooks and guestbook entries are stored on App Engine's data repository, <b>the High Replication Datastore (HRD) </b>
* The web framework used is webapp2, which interacts with the application via a WSGI interface.
* The use of Jinja2 as a templating engine is also demonstrated here.

<h3> Steps </h3>
* Create a folder for your application. In this case, it is <b>guestbook.</b> This is the directory which will be provided
  to the appcfg.py script when the app is to be deployed on to the App Engine.
* Each  App Engine application requires a configuration file, which, among other things, states the version number, the
  runtime environment, libraries etc. used in the application. 
  The syntax of the configuration file is [YAML-YAML Ain't Markup Language.](http://www.yaml.org/)
* There is another configuration file that is created, the index.yaml file in this case. This yaml file contains the 
  default index used by the data store queries. You can define a custom index for querying in this file.
* The main application content is written in guestbook.py script.
* The CSS stylesheet is defined in the stylesheets folder. The main.css stylesheet along with the index.html content is
  used by the jinja2 templating engine for formatting the web page output.



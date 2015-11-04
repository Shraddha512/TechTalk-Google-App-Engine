### High Level Report
===========

**What is Google App Engine?**

Google App Engine is a Platform as a Service (PaaS) offering that lets you build and run applications on Google’s infrastructure. App Engine applications are easy to build, easy to maintain, and easy to scale as your traffic and data storage needs change. With App Engine, there are no servers for you to maintain. You simply upload your application and it’s ready to go.

**App Engine Runtime Environment**

Google App Engine supports apps written in a variety of programming languages.

- Java: Using App Engine’s Java runtime environment, you can build your application using standard Java technologies.
- Python: App Engine features a fast Python interpreter and standard Python libraries.
- PHP: App Engine uses Google's Cloud Platform services under the hood when you call standard PHP functions.
- Go: App Engine features a Go runtime environment that runs natively compiled Go code.

**App Engine Development Environment**

Software Development Kits (SDKs) for App Engine are available in all supported languages. Each SDK includes:

- All of the APIs and libraries available to App Engine.
- A simulated, secure sandbox environment, that emulates all of the App Engine services on your local computer.
- Deployment tools that allow you to upload your application to the cloud and manage different versions of your application.

**Features**

| Feature        | Description    |
| :------------- | :------------- |
| App Identity   | A framework that provides access to the application's identity, and the ability to assert this identity using OAuth.     |
| Blobstore               | Allows your application to serve large data objects, such as video or image files, that are too large for storage in the Datastore service.               |
| Capabilities       | Detects outages and scheduled maintenance for specific services, so that an application may bypass them or notify users.   |
|Channel|Creates a persistent connection between your application and JavaScript clients, so you can send messages in real time without polling.|
|Datastore|A schemaless object datastore, with scalable storage, a rich data modeling API, and an SQL-like query language.|
|Datastore Backup/Restore|Allows you to export or import data to or from your application's Datastore using the Admin Console.|
|Dedicated Memcache|Provides a fixed cache capacity assigned exclusively to your application.|
|Go Runtime|	Build your application in the Go programming language.|
|Google Cloud Endpoints|	Generates APIs for Android, iOS, and web clients, making it easier to create a web backend for your app.|
|Google Cloud SQL|	A fully-managed web service that allows you to create, configure, and use relational databases that live in Google's cloud.|
|Google Cloud Storage Client Library|	Read and write to Google Cloud Storage, with internal error handling and retry logic.|
|HRD Migration Tool|	Migrates application data stored in the Blobstore or the deprecated Master/Slave Datastore into the GA High Replication Datastore.|
|Images|	Manipulate, combine, and enhance images. Converts between image formats, access image metadata such as height and frequency of colors.|
|Java Runtime| Build your application in the Java programming language.|
|Logs|	Programmatic access to application and request logs from within your application.|
|Mail|	Send email messages on behalf of administrators and users with Google Accounts, and receive mail at various addresses.|
|MapReduce|	An optimized adaptation of the MapReduce computing model for efficient distributed computing over large data sets.|
|Memcache|	A distributed, in-memory data cache that can be used to greatly improve application performance.|
|Modules|	Factor applications into logical components that can share stateful services and communicate in a secure fashion.|
|Multitenancy|	Makes it easy to compartmentalize your data to serve many client organizations from a single instance of your application.|
|OAuth|	Uses the OAuth protocol to provide a way for your app to authenticate a user who is requesting access without asking for credentials (username and password)|
|PHP Runtime|	Build your application in the PHP programming language.|
|Python Runtime|	Build your application in the Python programming language.|
|Remote	Access| App Engine services from any application. For example, access a production datastore from an app running on your local machine.|
|Scheduled Tasks|	Configure tasks that run at defined times or regular intervals.|
|Search|	Perform Google-like searches over structured data such as: plain text, HTML, atom, numbers, dates, and geographic locations.
SendGrid	Use SendGrid's library to send emails from your app and you can see statistics on opens, clicks, unsubscribes, spam reports and more.|
|Sockets|	Supports outbound sockets using the language-specific, built-in libraries.|
|SSL for Custom Domains|	Serve applications via HTTPS and HTTP from a custom domain rather than an appspot.com address.|
|Task Queue|	Allows applications to perform work outside of a user request, using small, discrete tasks, that are executed later.|
|Task Queue REST API|	Enables the use of an App Engine task queue over REST.|
|Task Queue Tagging|	Leases up to a specified number of tasks with the same tag from the queue for a specified period of time.|
|Traffic Splitting|	Routes incoming requests to different versions of your app, allowing you to do A/B testing and roll out new features incrementally.|
|Twilio|	Enables your application to make and receive phone calls, send and receive text messages, and make VoIP calls from any phone, tablet, or browser.|
|URL Fetch|	Uses Google's networking infrastructure to efficiently issue HTTP and HTTPS requests to URLs on the web.|
|Users|	Allows applications to sign in users with Google Accounts or OpenID, and address these users with unique identifiers.|
|XMPP|	Allows an application to send and receive chat messages to and from any XMPP-compatible chat messaging service.|

**Advantages**

- Infrastructure for Security: 
Around the world, the Internet infrastructure that Google has is probably the most secure. Google’s security and privacy policies are applicable to the apps developed using Google’s infrastructure.
- Scalability: 
Google creates its own apps using GFS, Big Table and other such technologies, which are available to you when you utilize the Google app engine to create apps. You only have to write the code for the app and Google looks after the testing on account of the automatic scaling feature that the app engine has.
- Performance and Reliability:
The app engine provides the same reliability and performance as any other Google product.
- Cost Savings:
You don’t have to hire engineers to manage your servers or to do that yourself. You can invest the money saved in to other parts of your business.
- Platform Independence:
You can move all your data to another environment without any difficulty as there is not much dependency on the app engine platform.

**Disadvantages**

- Limits the interaction with the underlying infrastructure. 
- Limits the languages it supports (can only use PHP, Python, Java and Go with App Engine) and integration with google cloud services is easy. 
- Shares the server with other products. So when some youtube servers are blocked it also blocks some of the shared App Engine server.
- Uses non relational database. Need to modify applications dependent on relational databses.



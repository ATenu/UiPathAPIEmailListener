# UiPath API - Email Listener Trigger
This python script works as an email listener that runs in background to catch new emails-trigger and use the content of those emails to interact with UiPath Orchestrator(Cloud) by using the Orchestrator API. Once an email containing a specific key value in the subject is received, a new element is created and added into a Queue stored in UiPath Orchestrator(Cloud).

How to use it:
1.1) Customize the configuration file (Config.json) by setting-up all the proper parameters.
1.2) Store the configuration file on the UiPathAPIEmailListener.py directory WITHOUT renaming it.
1.3) Import Requests 'pip install requests'
1.4) Run the script.

Orchestrator API calls used:
2.1) Authentication (POST) to request the "token"
2.2) Add Queue Item in a specific Queue

Info needed includes:
3.1) Client-ID
3.2) API Key (Refresh token)
3.3) OrganizationUnitID
3.4) Tenant Name
3.5) Logical Name
3.6) Queue Name

For more details on how to obtain all the data needed please refers to UiPath Documentantion and UiPath Swagger.

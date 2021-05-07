# UiPath API - Email Listener Trigger
This python script works as an email listener that runs in background to catch new emails-trigger and use the content of those emails to interact with UiPath Orchestrator(Cloud) by using the Orchestrator API. Once an email containing a specific key value in the subject is received, a new element is created and added into a Queue stored in UiPath Orchestrator(Cloud).

How to use it:
1) Customize the configuration file (Config.json) by setting-up all the proper parameters.
2) Store the configuration file on the UiPathAPIEmailListener.py directory WITHOUT renaming it.
3) Import Requests 'pip install requests'
4) Run the script.

Orchestrator API calls used:
1) Authentication to request the "token" (POST)
2) Add Queue Item in a specific Queue (POST)

Info needed also include:
1) Client-ID
2) API Key (Refresh token)
3) OrganizationUnitID
4) Tenant Name
5) Logical Name
6) Queue Name

For more details on how to obtain all the data needed please refers to UiPath Documentantion and UiPath Swagger.

# Business Process Management Labs
## Order Flow
### How to Start the Flows
-	Clone Repository
-	Start Eclipse and use the Repository as Workspace
-	Start Docker and wait until it is deployed and ready

If you want to use Sync:
-	Start OrderFlow.bpel with a correct Request (you can find an example in the request folder)

If you want to use Async:
-	Copy the ODE Port (in Eclipse: Simtech -> Preferences -> ODE)
-	Replace the callbackURL port in the Request with copied ODE Port
-	Start OrderFlow-async.bpel with a correct Request (you can find an example in the request folder)

After that you can use the WebGui.html.

If you open the html locally you have do deactivate the Chrome Security because of cross-domain-calls:  
chrome.exe --disable-web-security

URLs:   
http://46.101.159.46:[ODE-PORT]/ode/processes/OrderFlow   
http://46.101.159.46:[ODE-PORT]/ode/processes/OrderFlow-async
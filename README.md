# gitlab-webhooks-api

A Golang-based API and helper CLI system for:
-  Quickly building and using WebHook for automated deployment and operation and maintenance
-  Support: Github / GitLab / GitOsc,..etc
-  Config YAML file
-  SSH keys, API keys, ..etc on CLI ENV variables or YAML file. 
-  Supportfor Client/Server mode, and it can be used with the client to execute commands remotely without SSH.
-  Supports server based authentication when communicating with client for first time at Client/Server mode over WebSocket.
-  In Client/Server mode, x-smarthook-tokenrequest headers to authenticate the client connection.
-  Hooks a main messaging service for notification 


The interface and development ideas refer to git-webhook .https://docs.gitlab.com/ee/user/project/integrations/webhooks.html
 
You can use PushSafer Chrome extension from https://www.pushsafer.com/ for testing/debugging

On the basis of the other reference project, the relationship between server based WebHook and Server is decoupled, and a many-to-many relationship is realized.
Because SSH method to be used to communicate with the server, please keep the server account and password.



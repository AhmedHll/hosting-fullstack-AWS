### **Pipeline diagram.**
[link](https://lucid.app/lucidchart/29ad73f4-8141-4ddd-b97a-a65d4bcb575d/edit?beaconFlowId=AE7BD82D01E8FEFC&invitationId=inv_92c00606-5cef-45bd-b5bd-b7a832c403b8&page=0_0#)
![Pipeline diagram](/screenshots/pipeline-daigram.png?raw=true "Optional Title")

##Pipeline process

* first install node and checkout code
* then setup aws-cli
* use root level package.json to install dependencies in the frontend app

-
1- job one (Build)
 * npm run api:install
 * npm run frontend:build
 * npm run api:build

2- job two (Deploy)
 * npm run deploy to run command > 'npm run api:deploy && npm run frontend:deploy'

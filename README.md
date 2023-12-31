# homeassistantKmlFlow
Node-Red Flow to create a KML Network Link of Home Assistant Entity locations.

![flow](/homeassistantKmlFlow.png?raw=true "Node Red Flow")

![flow](/homeassistantATAK.png?raw=true "ATAK")


SETUP HOME ASSISTANT SERVER:

-https://www.home-assistant.io/installation/

-options include installing and hosting Home Assistant on a Raspberry Pi or similar single board computer or mini PC, buying dedicated hardware running Home Assistant, deploying Home Assistant on a cloud server or virtual private server (VPS), Docker Container, or local virtual environment. Just note the Home Assistant server software you are using since certain features are only available to Home Assistant deployments (ie: home assistant core vs home assistant OS vs home assistant supervised vs home assistant container)

----------------------------------------------

SETUP NODE-RED:

-https://nodered.org/docs/getting-started/

-options include installing node-red on your local PC, a Raspberry Pi or similar single board computer or mini PC, deploying node-red on a cloud server or virtual private server (VPS), Docker Container, or local virtual environment. After installing node-red you should be able to go to the node-red dashboard at http://node-red-ip-address:1880 you may have to open appropriate ports (1880) to allow devices to access the node-red dashboard.

----------------------------------------------

IMPORT .JSON FLOW TO NODE RED:

-in GitHub: click on "homeassistantKmlFlow.json" > click on the download icon "Download raw file" > note where the homeassistantKmlFlow.json file downloaded to, default is in your Downloads folder

-in Node-Red: click on menu icon (3 horizontal lines top right) > click on "Import" > click on "select a file to import" > go to Downloads folder and click on "homeassistantKmlFlow.json" > Upload > Import


ALTERNATIVELY..

-you can just copy the whole "homeassistantKmlFlow.json" code from GitHub and paste it into the Node-Red Import Clipboard.

----------------------------------------------

GETTING HOME ASSISTANTS API ACCESS TOKEN:

-In HomeAssistant: scroll down and click on your profile > scroll down to "Long-Lived Access Tokens" > click on "CREATE TOKEN" > give your token a name > copy your access token

-In Node-Red: go to "homeassistantKmlFlow" flow > click on "http req" node > check mark "Use authentication" > Type: bearer authentication > Token: *paste your access token here

----------------------------------------------

ACCESSING THE KML NETWORK LINK:

-the default kml network link for the "homeassistantKmlFlow" is http://node-red-ip-address:1880/homeassistant.kml

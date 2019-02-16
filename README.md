# Sample-Accounts-LWC Lightning Web Component
Sample Lightning Web component showing uses of Lightning Data Table, Displaying Lookup fields data in Data Table, Lightning Record Form, Lightning Map and how to call an apex class to get list of accounts.

## Demo
<img src="https://github.com/thatherahere/Sample-Accounts-LWC/blob/master/demo.gif"/>

## Installing using Salesforce DX

1. Set up your environment. Follow the steps in the [Quick Start: Lightning Web Components](https://trailhead.salesforce.com/content/learn/projects/quick-start-lightning-web-components/) Trailhead project. The steps include:

    - Sign up for a Spring '19 pre-release org and enable Dev Hub
    - Install the pre-release version of the Salesforce CLI
    - Install Visual Studio Code
    - Install the Visual Studio Code Salesforce extensions, including the Lightning Web Components extension

1. If you haven't already done so, authenticate with your Spring '19 hub org and provide it with an alias (devhub):

    ```
    sfdx force:auth:web:login -d -a devhub
    ```

1. Clone the repository:

    ```
    git clone https://github.com/thatherahere/Sample-Accounts-LWC.git
    cd Sample-Accounts-LWC
    ```

1. Create a scratch org and provide it with an alias (lwcdemo):

    ```
    sfdx force:org:create -s -f config/project-scratch-def.json -a lwcdemo
    ```

1. Push the app to your scratch org:

    ```
    sfdx force:source:push
    ```

1. Assign the **Custom_Permissions** permission set to the default user:

    ```
    sfdx force:user:permset:assign -n Custom_Permissions
    ```

1. Load sample account records:

    ```
    sfdx force:data:tree:import --plan ./data/data-plan.json
    ```

1. Open the scratch org:

    ```
    sfdx force:org:open
    ```
1. In App Launcher, select the **Sample LWC** tab.

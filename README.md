# devops-demo-sample-ace-project
ACE Toolkit Workspace for sample application

## Creating a workspace folder from IBM App Connect Enterprise

1. Set up your base workspace folder at Enterprise startup
<img src="Images/01-set-wrkspc-fldr.png" width="550">

2. Create a new REST API
<img src="Images/02-new-api.png" width="250">

3. Set up your project name. See the warning below about naming convention.
<img src="Images/03-set-prjt-name.png" width="450">

4. Import the API via a json file. The one shown is from swagger.
<img src="Images/04-set-json.png" width="550">

5. Once the JSON is imported, click on the create subflow button.
<img src="Images/05-set-subflows.png" width="750">

6. Since we created this project with a JSON file, we can, in this step, invoke a rest operation based on the json file embedded in the project.
<img src="Images/06-ref-swagger2.png" width="750">

7. This is where the embedded file should be kept.
<img src="Images/07-ref-swagger3.png" width="750">

8. Once we select the embedded json, we select the action we want to invoke for the subflow. In this case, it is the get operation for the inventory.
<img src="Images/08-select-action.png" width="750">

9. Click on RESTRequest under the REST tab and drag it onto the main window.
<img src="Images/09-new-request.png" width="250">

10. Connect the input to the input of the get action icon and connect the output tab of the action to the output.
<img src="Images/10-connect-dots.png" width="650">

11. For the action icon properties, set the Base URL Override to the base url set for the inventory.
<img src="Images/11-url-override.png" width="650">

```
### Warning:
When creating the project name, please use only lowercase letters and dashes only. Failure to do so will result in an unsuccessful deployment of the ace server.

3. Click on the link to the newly executed PipelineRun and monitor the status.  You can also run `oc get pods -w` in the <project> to view the status of the pods.
```

Test 6

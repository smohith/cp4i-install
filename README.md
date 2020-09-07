# Installing Cloud Pak for Integration
The IBM Cloud Pak for Integration (CP4I) is delivered as operators that are installed and managed using the Operator Lifecycle Manager (OLM) within Red Hat OpenShift. To install CP4I, we will verify that the OLM Catalog Sources for IBM components have been added, we will then install the operators using OLM, create the CP4I custom resource, and finally deploy some of the capabilities and runtimes.

### OLM Catalog Sources
1. From your web browser use the bookmark tab to open the OpenShift console.
2. The login credentials should already be saved in the browser. If not use `ibmuser` as Username and `engageibm` as Password.
3. From the left hand menu expand `Operators > OperatorHub` and search for `cloud pak`. If the result is similar to the screenshot below skip Step 4 below.

   ![operators.png](images/operators.png)

4. (Optional) Click on the ![plus.png](images/plus.png) sign in the top right hand corner and paste the code from ![cs.yaml](code/cs.yaml) in the yaml editor and click `Create`. Repeat with ![cp.yaml](code/cp.yaml). Within a few minutes there should be two new pods in the `openshift-marketplace` project.

   ![operator-pods.png](images/operator-pods.png)

5. 



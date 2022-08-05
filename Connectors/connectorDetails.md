---
layout: page
title: Connectors Details
---

# GitHub MERN Stack Repository Connector

In the Harness CI module user interface, click *New Connector*.

![](../assets/images/image006.jpg)

Select *GitHub*

![](../assets/images/image013.jpg)

Enter “MERN Stack Example” in the Name field, then click Continue.

![](../assets/images/image014.jpg)

Select **Repository** for **URL Type**.

Select **HTTP** for **Connection Type.**

Enter the url of your MERN Stack Example repoin the **GitHub Repository URL** field. Then click **Continue**.

![](../assets/images/image015.jpg)
 

Enter your GitHub username in the **Username** field, then click **Create or Select a Secret**.

![](../assets/images/image016.jpg)

Select **GitHub Personal Access Token**, then click **Apply Selected**.

![](../assets/images/image017.jpg)

Verify that **GitHub Personal Access Token** appears in the **Personal Access Token** field. Then click Continue.
 
![](../assets/images/image018.jpg)

Select **Connect through a Harness Delegate**, then click Continue.

![](../assets/images/image019.jpg)

Select **Only use Delegates with all of the following tags**. Then select **mern-demo** from the drop-down menu.

Click **Save and Continue**.
 
 ![](../assets/images/image020.jpg)

A connection test will run, when you see Verification successful, click Finish.

![](../assets/images/image021.jpg)
 
# GitHub MERN Stack Example GitOps Repository

Click New Connector.
 
![](../assets/images/image006.jpg)

Select *GitHub*

![](../assets/images/image013.jpg)

Enter “MERN Stack Example GitOps” in the **Name** field, then click **Continue**.

![](../assets/images/image022.jpg)

Select **Repository** for **URL Type**.

Select **HTTP** for **Connection Type**.

Enter the url for your GitOps clone in the **GitHub Repository URL** field. Then click **Continue**.

![](../assets/images/image023.jpg)

Enter your GitHub username in the **Username** field, then click **Create or Select a Secret**.
 
![](../assets/images/image016.jpg)

Select **GitHub Personal Access Token**, then click **Apply Selected**.

![](../assets/images/image017.jpg)

Verify that **GitHub Personal Access Token** appears in the **Personal Access Token** field. Then click **Continue**.

![](../assets/images/image018.jpg)

Select Connect through a Harness Delegate, then click Continue.
 
![](../assets/images/image019.jpg)

Select **Only use Delegates with all of the following tags**. Then select **mern-demo** from the drop-down menu.

Click Save and Continue.

![](../assets/images/image020.jpg)

A connection test will run, when you see Verification successful, click Finish.
 
![](../assets/images/image021.jpg)

# Kubernetes Cluster

Click **New Connector**.
 
![](../assets/images/image006.jpg)

Select **Kubernetes Cluster**.
 
![](../assets/images/image024.jpg)

Enter “My Cluster” in the Name field, then click **Continue**.
 
![](../assets/images/image025.jpg)

Select **Use the credentials of a specific Harness Delegate**, then click **Continue**.
 
![](../assets/images/image026.jpg)

Select **Only use Delegates with all of the following tags**. Then select **mern-demo** from the drop-down menu.

![](../assets/images/image027.jpg)

Click **Save and Continue**.
 
![](../assets/images/image028.jpg)

Wait for the test to complete, then click **Finish**.

# All done with Connectors!

<a class="btn btn-primary" href="../Connectors/connectorDetails">Can I go back to the connectors intro please?</a>
<a class="btn btn-primary" href="../Services/servicesIntroduction">✅ Onward and Upwards to Services</a>
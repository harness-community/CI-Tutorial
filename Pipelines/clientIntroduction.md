---
layout: page
title: Client Pipeline Introduction
---

## MERN Client CI Pipeline

Click **New Pipeline**.

![](../assets/images/image061.jpg)

Enter “Build MERN Client” in the **Name** field, then click **Start**.

![](../assets/images/image062.jpg)

### Stage

Click **Add Stage**, then select **Build**.

![](../assets/images/image037.jpg)

Enter “MERN Client” in the **Stage Name** field, then click **Select Connector**.

![](../assets/images/image063.jpg)

Select **MERN Stack Example**, then click **Apply Selected**.

![](../assets/images/image039.jpg)

Verify that MERN Stack Example appears in the Connector field, then click Set Up Stage.

![](../assets/images/image064.jpg)

Verify that MERN Client appears in the Name field, then click Continue.

![](../assets/images/image065.jpg)

select **Hosted by Harness** and then click **start provisioning**.

![](../assets/images/image042.jpg)

And you’re done with the delegate.

### Build Step

Click **Add step**.

![](../assets/images/image044.jpg)

Select **Build and Push an image to Docker Registry**.

![](../assets/images/image050.jpg)

Enter “Client Docker Image” in the **Name** field.

Click **Select** in the **Docker Connector** field.

![](../assets/images/image066.jpg)

Select **Docker Hub**, then click **Apply Selected**.

![](../assets/images/image052.jpg)

Verify that **Docker Hub** appears in the **Docker Connector** field.

Enter “dockerusername/mern-client” in the **Docker Repository** field. Replacing “dockerusername” with your Docker Hub username. Then click **Add**.

![](../assets/images/image067.jpg)

Enter ```<+pipeline.sequenceId>``` in the **Tag** field, then click **Optional Configuration**.

![](../assets/images/image054.jpg)

Enter “client/Dockerfile” in the **Dockerfile** field.

Enter “client” in the **Context** field, then click **Add** under **Build Arguments**.

![](../assets/images/image068.jpg)

Enter “SERVER_URI” in the first field. Then select Runtime input from the drop-down menu in the second field.

![](../assets/images/image069.jpg)

Verify the **SERVER_URI** build argument value shows **<+input>**.

Enter “2000Mi” in the **Limit Memory** field.

![](../assets/images/image070.jpg)

Click **Apply Changes**.

![](../assets/images/image071.jpg)


### Run Pipeline

Click **Save**.

![](../assets/images/image057.jpg)

Click Run.

![](../assets/images/image058.jpg)

Select **Git Branch** for **Build Type**.

Enter “main” in the Branch Name field.

Enter your MERN Server’s URI in the **SERVER_URI** value field. This will be the external IP of the server retrieved with kubectl in the previous step. In this example, the MERN Server’s URI is `http://34.75.52.141:5001`, replace `34.75.52.141` with your MERN Server’s external IP.

Click Run Pipeline.

![](../assets/images/image072.jpg)

Now that you’ve built the images, tested them and pushed them to Docker Hub, you are ready to deploy into production. That’s where continuous delivery comes in. To continue your journey, check out the second part of this series, Harness CD for MERN Stack Example.
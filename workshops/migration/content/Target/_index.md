+++
title = "Updating the Target Workload"
date = 2020-08-07T14:42:38-04:00
weight = 6
chapter = true
pre = "<b>6. </b>"
+++

# Updating the Target Workload

In this exercize, we will add the application and underlying host of the recently deployed Wordpress stack in US West 2 into the empty target workload that Nimbus created for us previously. This process will be nearly identical to the *Creating a Workload* step you completed earlier.

Open up the browser tab to the target workload Overview page and click on the **Edit workload** link at the top right hand corner of your screen:

![alt text](/images/edit-workload.png "Edit Workload")

In the search bar, type in **php** and press Enter on your keyboard.  Click on the **+** icons next to the two entries for **PHP Application**: ***Service*** and ***Browser application***. (Applications in New Relic are referred to as services) Then, click on the **Save changes** button on the bottom right hand side of your screen.

![alt text](/images/entity-search.png "Entity Search")

If you click on the **Entities** tab near the top left hand side of your screen, you should now see the two entities you just added to your Workload:

![alt text](/images/entity-list-1.png "Entity Listing")

***Since we didn't name the application deployed in US West 1 differently than that of the application deployed in US West 2, New Relic treats them as the same application running on separate host instances.***

Click back over to the **Overview** tab and click on the **Edit workload** link once again.  This time, type **Host** into the search bar, wait for the *Hosts ENTITY TYPE* recommendation in the dropdown, and then select it:

![alt text](/images/search-for-hosts.png "Host Entities")

If you created a new AWS account for this workshop, you should now see two hosts listed: one for each AWS region that you have deployed the Wordpress stack in.  Click the **+** icon next to the instance deployed in US West 2, followed by clicking the **Save changes** button to add it to your Workload:

![alt text](/images/add-host.png "Add Host")

If you are using an AWS account with other running instances, you can locate the instance for this Workshop by visting the [Stacks](https://console.aws.amazon.com/cloudformation/home?region=us-west-1#/stacks?filteringText=&filteringStatus=active&viewNested=true&hideStacks=false) page and clicking on the link of the stack name you created for this Workshop (*New-Relic-Wordpress*):

![alt text](/images/locate-stack.png "Locate Stack")

You can then click on the **Resources** tab and click on the link provided under the *Physical ID* column for the *WebServer* that was launched by the template:

![alt text](/images/instance-details.png "Instance Details")

By default, your instance hostname will be determined by its private IP:

![alt text](/images/private-ip.png "Private IP")

Once you have successfully added the host to your Workload, you should be presented with an overview page that looks similar to the one below:

![alt text](/images/workload-overview.png "Workload Overview")

Congratulations!  You have successfully updated your target Workload.  You may now move on to the next step in this Workshop.

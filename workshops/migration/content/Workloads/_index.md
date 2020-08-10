+++
title = "Creating a Workload"
date = 2020-08-06T15:05:22-04:00
weight = 3
chapter = true
pre = "<b>3. </b>"
+++

# What is a Workload?

New Relic's Workloads feature gives you the ability to group and monitor [entities](https://docs.newrelic.com/docs/new-relic-one/use-new-relic-one/core-concepts/what-entity-new-relic) based on a team or a set of responsibilities, from front-end to back-end services, across your entire stack.

Workloads help you understand complex systems, detect issues, understand the cause and impact of an incident, and resolve those issues quickly.

When migrating applications to the cloud, New Relic recommends that you group all of your software stacks into Workloads.  

In this Workshop, we will be creating a single Workload from our application and underlying host instance and migrating it from one AWS region to another.

# Creating a Workload

Open the New Relic One [Workloads](https://one.newrelic.com/launcher/workloads.home) application and click on the **Create a workload** button located at the top right hand corner of your screen.

![alt text](/images/create-a-workload.png "Create a Workload")

Give your Workload a name (we recommend *New-Relic-Wordpress*) and click the **Create a workload** button on the bottom right hand side of your screen:

![alt text](/images/name-your-workload.png "Name your Workload")

Click on the **Add entities** link located near the top right hand portion of your screen:

![alt text](/images/add-entities.png "Add Entities")

In the search bar, type in **php** and press Enter on your keyboard.  Click on the **+** icons next to the two entries for **PHP Application**: ***Service*** and ***Browser application***. (Applications in New Relic are referred to as services) Then, click on the **Save changes** button on the bottom right hand side of your screen.

![alt text](/images/entity-search.png "Entity Search")

If you click on the **Entities** tab near the top left hand side of your screen, you should now see the two entities you just added to your Workload:

![alt text](/images/entity-list-1.png "Entity Listing")

Click back over to the **Overview** tab and once again click on the **Add entities** link.  This time, type **Host** into the search bar, wait for the *Hosts ENTITY TYPE* recommendation in the dropdown, and then select it:

![alt text](/images/search-for-hosts.png "Host Entities")

If you created a new AWS account for this workshop, you should only see one host listed.  Click the **+** icon, followed by clicking the **Save changes** button to add it to your Workload:

![alt text](/images/add-host.png "Add Host")

If you are using an AWS account with other running instances, you can locate the instance for this Workshop by visting the [Stacks](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks?filteringText=&filteringStatus=active&viewNested=true&hideStacks=false) page and clicking on the link of the stack name you created for this Workshop (*New-Relic-Wordpress*):

![alt text](/images/locate-stack.png "Locate Stack")

You can then click on the **Resources** tab and click on the link provided under the *Physical ID* column for the *WebServer* that was launched by the template:

![alt text](/images/instance-details.png "Instance Details")

By default, your instance hostname will be determined by its private IP:

![alt text](/images/private-ip.png "Private IP")

Once you have successfully added the host to your Workload, you should be presented with an overview page that looks similar to the one below:

![alt text](/images/workload-overview.png "Workload Overview")

Congratulations!  You have successfully created a New Relic Workload.  You may now move on to the next step in this Workshop.

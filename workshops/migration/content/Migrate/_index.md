+++
title = "Migrating a Workload"
date = 2020-08-07T11:34:24-04:00
weight = 4
chapter = true
pre = "<b>4. </b>"
+++

# Migrating a Workload

New Relic provides an application named **Nimbus** that allows you to track the migration of your Workloads in real time.  Normally, you'd use Nimbus to create Workloads from your on-prem estate and migrate them to a cloud provider such as AWS.  In this Workshop however, we will simply be migrating the Workload we have created from one AWS region to another.

Let's start by **opening Nimbus** and clicking on the **Migrate Workloads** link in *Getting Started* menu near the top left hand side of your screen:

![alt text](/images/nimbus-migrate-workloads.png "Migrate Workloads")

You should see the **New-Relic-Wordpress** Workload listed that we created in the previous step in this Workshop. Click the green **Migrate** button:

![alt text](/images/nimbus-select-workload.png "Select Workload")

In the popup dialog you are presented with, select your New Relic acocunt name from the first dropdown box while ensuring the other dropdowns match what you see in the screenshot below, then click the green **Create Project** button:

![alt text](/images/nimbus-create-project.png "Create Project")

When you clicked on the **Create Project** button in the previous step, Nimbus automatically created an empty, *target* Workload that it will use to track your migration progress.  Open this Workload by clicking on the link provided in the *Target* column of your Workload listing:

![alt text](/images/nimbus-target-workload.png "Target Workload")

***Make sure to keep the target Workload browser tab open as we will be revisiting it later in this Workshop.***

Congratulations!  You have successfully prepared your Workload for migration and may now move on to the next step in this Workshop.

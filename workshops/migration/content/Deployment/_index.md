+++
title = "Deployment - US East 1"
date = 2020-08-06T10:05:24-04:00
weight = 2
chapter = true
pre = "<b>2. </b>"
+++


# Deployment - US East 1

First, [download](http://emea-partners.newrelic-es.com/lab1_NewRelic-WP-Infra-APM.template) the CloudFormation template that will be used to deploy your Wordpress stack. Then, in [CloudFormation](https://console.aws.amazon.com/cloudformation/home?region=us-east-1), from the  **Create Stack** dropdown menu, select **With new resources (standard)**.  The CloudFormation link above will launch this CloudFormation stack in the US East 1 AWS region.  ***Do not choose a different region. You will also need to create a [key pair](https://console.aws.amazon.com/ec2/v2/home?region=us-east-1#KeyPairs:) in this region before proceeding.***

![alt text](/images/cf-dropdown.png "CloudFormation")

## Create Stack Wizard - Step 1

In the Create Stack wizard, select the **Upload a template file** radio button, and then provide the CloudFormation template you recently downloaded by clicking on **Choose File**:

![alt text](/images/create-stack-wizard.png "Create Stack")

Once you have selected the *lab1_NewRelic-WP-Infra-APM.template* CloudFormation template from the file dialog, you should be returned to the Create Stack Wizard.  Click the orange **Next** button on the bottom right hand side of your screen.

## Create Stack Wizard - Step 2

You will now need to name your stack; we recommend using *New-Relic-Wordpress* as that is the name that will be used in the example screenshots below:

![alt text](/images/stack-name.png "Stack Name")

Next, you will choose a key pair from the first dropdown menu in the *Parameters* section of the wizard:

![alt text](/images/select-key-pair.png "Select Key Pair")

Now, you will need to provide your [New Relic license key](https://docs.newrelic.com/docs/accounts/accounts-billing/account-setup/new-relic-license-key#finding):

![alt text](/images/new-relic-license-key.png "New Relic License Key")

Lastly, provide the username and password parameters needed by Wordpress and click the orange **Next** button on the bottom right hand side of your screen:

![alt text](/images/wordpress-params.png "Wordpress Parameters")

## Create Stack Wizard - Step 3

Nothing needs to be configured in step 3 of the Create Stack Wizard;  simply scroll down and click the orange **Next** button on the bottom right side of your screen.

## Create Stack Wizard - Step 4

Review the parameters you have provided to see if you have made any obvious errors.  If not, simply scroll down and click the orange **Create stack** button on the bottom right side of your screen.

## Verification

Before moving on in the Workshop, ensure your Wordpress stack was launched successfully by visiting the [Stacks](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks?filteringText=&filteringStatus=active&viewNested=true&hideStacks=false) page.  You should see a green entry **CREATE_COMPLETE** in the status column for your stack.  This can take a few minutes, so refresh the page periodically until the process has completed. 


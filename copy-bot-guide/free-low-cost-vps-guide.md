# Free/Low-Cost VPS Guide

### Google Cloud VPS <a href="#google-cloud-vps" id="google-cloud-vps"></a>

Google Cloud offers a free tier VPS: [https://cloud.google.com/free/docs/gcp-free-tier](https://cloud.google.com/free/docs/gcp-free-tier)

In this guide, we will show you how to configure your Google Cloud free tier VPS. As long as you stay within the free tier limits, your access will never expire. Unlike some other services such as AWS, you will not lose access at the end of the trial period.

You will need to sign up for a Google Cloud account and create a new project:

In order to get access to Google Cloud free tier VPS, you will need to set up a billing account and add your credit card information. Return to your project and associate your project with the new billing account you have created.

Then you can go to Compute Engine and create a new VM instance:

You will need to configure your VM instance to comply with the free tier limits if you do not want to be charged. You will be able to run one VM instance for free: [https://cloud.google.com/free/docs/free-cloud-features#free-tier-usage-limits](https://cloud.google.com/free/docs/free-cloud-features#free-tier-usage-limits)

For the VPS region, make sure you select only Oregon, Iowa, or South Carolina:

Under Presets, you should choose the e2-micro VM. This is the only option that qualifies for the free tier:

Next, under Boot Disk, you should change the default options and select a 30GB standard persistent disk:

Finally, under Firewall, you should allow HTTP and HTTPS traffic. This will allow you to connect with your RPC node, access the internet, and send transactions.

You will see that there is an estimated monthly charge for the VPS, but you don't need to worry. As long as you are only running a single VPS instance and you have configured the VPS according to the free tier usage limits, you will not be charged.

### Oracle Cloud VPS <a href="#oracle-cloud-vps" id="oracle-cloud-vps"></a>

Oracle Cloud is also another alternative option for a free VPS: [https://www.oracle.com/cloud/free/](https://www.oracle.com/cloud/free/)

You will need to sign up for an account and add your credit card number for access to the free tier VPS. We recommend using Oracle Cloud VPS over Google Cloud VPS because they provide several locations near Jito BlockEngines, including Frankfurt, London, Amsterdam, Tokyo.

You will first be asked to provide your name and e-mail. After you verify your e-mail address you can create your Oracle Cloud Account. You should pay special attention to this section because you will only be allowed to choose one home region and you will not be allowed to change it. Make sure to choose a home region that is located in one of the Jito BlockEngine cities before proceeding to the next step.

In the next section, you will be asked to entire your name, address, phone number, and credit card information. Once that is complete, you can start your trial. You will be asked to setup two-factor authentication for your login.

On your dashboard, you should click on Instances in the Pinned Service Links.

On the next page, click Create Instance.

You can check the details of your VPS instance. Make sure that you have selected options that are Always Free-eligible if you do not wish to be charged.

You can confirm the estimated price estimate. Similar to Google Cloud, this is only an estimate and if you stay within the free tier limits, you will not be charged. Once you are done, you can click Create to finish your VPS setup.

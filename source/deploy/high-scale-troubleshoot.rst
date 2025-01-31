Troubleshooting high scale deployments
=======================================

This page provides troubleshooting guidance for high scale Mattermost deployments with 100 users or more.

If these steps do not resolve the issue, and you have a `paid subscription to a Mattermost offering </about/editions-and-offerings.html>`_, please reach out to our customer support team via our `online support portal <https://support.mattermost.com/hc/en-us/requests/new>`_. 

Additionally, peer-to-peer support is available for all Mattermost users in our `troubleshooting forum <https://forum.mattermost.com/c/trouble-shoot>`__ and on our `community server <https://community.mattermost.com/core/channels/peer-to-peer-help>`_. 

My system keeps hanging when I search for a message in Mattermost
---------------------------------------------------------------------

First, check how many messages have been posted on your system, including deleted posts and posts made using automations.

Go to the **System Console > Reporting > Site Statistics** and review the **Total Posts** figure reported. If this figure is above 3,000,000 posts, we recommend deploying Elasticsearch alongside your Mattermost server for improved search performance. Follow our guides to `deploy an Elasticsearch server </scale/elasticsearch.html>`__.
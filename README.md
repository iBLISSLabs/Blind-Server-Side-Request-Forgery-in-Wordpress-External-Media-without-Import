# Blind Server Side Request Forgery (SSRF) in Wordpress External Media without Import

This PoC describe how to exploit a Blind SSRF in - Wordpress External Media without Import version 1.1.2

# Description

The External Media without Import v1.1.2, plugin for Wordpress does not have protections against SSRF, so it is possible to forge requests to internal services that are not directly exposed, if you know the path.

![image](https://user-images.githubusercontent.com/70114276/160252778-e20b6a65-b111-446c-ae11-a944246b834c.png)

## Attack Scenario

![image](https://user-images.githubusercontent.com/70114276/160253730-f565d8de-158f-4596-9eb5-9d931fb1d692.png)

After trying to directly access the service, we are not successful

![image](https://user-images.githubusercontent.com/70114276/160253917-67d86a0d-a9ef-499f-b660-45bf18556550.png)

So we can perform a fake requests with this plugin through the add an image function

![image](https://user-images.githubusercontent.com/70114276/160254035-6bb3a72d-c525-4e41-94a4-9caac749ba28.png)

![image](https://user-images.githubusercontent.com/70114276/160254182-b632ba37-45d3-4ea5-a9f5-0cd3aa3c7883.png)

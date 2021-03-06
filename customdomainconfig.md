---

copyright:
  years: 2016, 2018
lastupdated:  "2018-11-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock:  .codeblock}

# Configuring custom domain for Mobile Foundation server
{: #configcustomdomain}

{{site.data.keyword.mobilefoundation_short}} creates a {{site.data.keyword.mfserver_short_notm}}, which is accessible using a URL with the domain names based on the {{site.data.keyword.Bluemix_notm}} **Region**. You can also configure your own custom domain.
{: shortdesc}

The URL or route is created with the default domain names based on the {{site.data.keyword.Bluemix_notm}} `Region`.

  |Domain |  Region  |    
  |:----- | :----- |    
  |`mybluemix.net` | US South |    
  |`eu-gb.mybluemix.net` | United Kingdom  |
  |`au-syd.mybluemix.net` | Sydney  |   
  |`eu-de.mybluemix.net` | Frankfurt |   
  {: caption="Table 1. Application domain names based on Region in {{site.data.keyword.Bluemix_notm}}" caption-side="top"}

To be able to use your own domain, you'll need to configure custom domain by performing the following steps:

1.	Create a {{site.data.keyword.mfserver_short_notm}} instance  by creating the {{site.data.keyword.mobilefoundation_short}} service instance by choosing one of the supported plans.

+ Add the custom domain that you would want to use, to your {{site.data.keyword.Bluemix_notm}} `Organization`. Go to **Manage Organizations > DOMAINS > ADD DOMAIN** to add your own domain.

+ Set up a route for the server to use your custom domain.

+ Go to the DNS provider for your domain, and add a CNAME entry, which will route the traffic from your domain to the default {{site.data.keyword.Bluemix_notm}} route, where the server is running.

+ If you would like to configure `https` for your custom domain, then upload the SSL certificate for your domain in {{site.data.keyword.Bluemix_notm}}. To do this go to **Manage Organizations > DOMAINS**, select the custom domain you want to configure SSL certificate for, click the **Upload Certificate** to upload SSL certificate for your domain. Refer to [this post ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://developer.ibm.com/bluemix/2014/09/28/ssl-certificates-bluemix-custom-domains/){: new_window}, for more information.

---

copyright:
  years: 2016, 2018
lastupdated:  "2018-11-19"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock:  .codeblock}

# Configuración de un dominio personalizado para el servidor Mobile Foundation
{: #configcustomdomain}

{{site.data.keyword.mobilefoundation_short}} crea un {{site.data.keyword.mfserver_short_notm}}, que es accesible mediante un URL con los nombres de dominio basados en la **Región** de {{site.data.keyword.Bluemix_notm}}. También puede configurar su propio dominio personalizado.
{: shortdesc}

El URL o la ruta se crean con los nombres de dominio predeterminados basados en la `Región` de {{site.data.keyword.Bluemix_notm}}.

  |Dominio |  Región  |    
  |:----- | :----- |    
  |`mybluemix.net` | EE.UU. sur |    
  |`eu-gb.mybluemix.net` | Reino Unido  |
  |`au-syd.mybluemix.net` | Sídney  |   
  |`eu-de.mybluemix.net` | Frankfurt |   
  {: caption="Tabla 1. Nombres de dominio de aplicación basados en Región en {{site.data.keyword.Bluemix_notm}}" caption-side="top"}

Para poder utilizar su propio dominio será necesario configurar el dominio personalizado realizando los siguientes pasos:

1.	Cree una instancia de {{site.data.keyword.mfserver_short_notm}} creando la instancia de servicio de {{site.data.keyword.mobilefoundation_short}} seleccionando uno de los planes soportados.

+ Añada el dominio personalizado que desea utilizar a la `Organización` de {{site.data.keyword.Bluemix_notm}}. Vaya a **Gestionar organizaciones > DOMINIOS > AÑADIR DOMINIO** para añadir su propio dominio.

+ Configure una ruta para que el servidor utilice el dominio personalizado.

+ Vaya al proveedor DNS para su dominio y añada una entrada CNAME, que dirigirá el tráfico de su dominio a la ruta de {{site.data.keyword.Bluemix_notm}} predeterminada, donde se está ejecutando el servidor.

+ Si desea configurar `https` para el dominio personalizado, cargue el certificado SSL para su dominio en {{site.data.keyword.Bluemix_notm}}. Para hacerlo, vaya a **Gestionar organizaciones > DOMINIOS**, seleccione el dominio personalizado para el que desea configurar el certificado SSL, pulse **Cargar certificado** para cargar el certificado SSL para su dominio. Consulte [esta publicación ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://developer.ibm.com/bluemix/2014/09/28/ssl-certificates-bluemix-custom-domains/){: new_window} para obtener más información.

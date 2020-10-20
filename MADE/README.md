# CustomFontsSAC

Demo repository to showcase usage of custom icon fonts in SAC.br
The `gh-pages` branch hosts the SAP Fiori icon font released with [OpenUI5](httpsopenui5.org).

 Note For demonstration purposes only, we use the `gh-pages` branch to host the custom font definition files. Be advised that this is not recommended for productive use. You can host the files similarly on any kind of publicly available webserver or cloud infrastructure, though.

## Instructions

1. To use the SAP Fiori Icon Font in SAP Analytics Cloud, host a simple [font definition file](httpsmichadelic.github.ioCustomFontsSACSAP-icons.css) on a public server

 ``` css
  SAP Fiori Icons 
 @font-face {
   font-family 'SAP Fiori Icons';
   src
     url('httpsyourserverpathtoSAP-icons.woff2') format('woff2'),
     url('httpsyourserverpathtoSAP-icons.woff') format('woff'),
     url('httpsyourserverpathtoSAP-icons.ttf') format('truetype');
   font-weight normal;
   font-style normal;
 }
 ```

2. Download the three font files `sap-icons.ttf`, `sap-icons.woff`, `sap-icons.woff2` from the latest UI5 shipment and put it right next to the definition file.

    [SAP-Icons.woff2](httpssapui5.hana.ondemand.comresourcessapuicorethemesbasefontsSAP-icons.woff2)
    [SAP-Icons.woff](httpssapui5.hana.ondemand.comresourcessapuicorethemesbasefontsSAP-icons.woff)
    [SAP-Icons.ttf](httpssapui5.hana.ondemand.comresourcessapuicorethemesbasefontsSAP-icons.ttf)

3. Add the font definition URL to the SAC custom web font settings (see documentation link below).

   ![Add font definition](imagesaddFont.png)

4. Add the hostname where the font is located to the Trusted Origins in the SAP Analytics Cloud Administration page.

   ![Add trusted origin](imagestrustedOrigin.png)

5. Done! You are now ready to use the SAP Fiori icon font in your SAP Analytics Cloud stories

   ![Use custom icon](imagescustomIcon.png)

## Related Information

 [SAP Fiori Iconography](httpsexperience.sap.comfiori-design-webicons) The SAP Fiori design guidelines for icons
 [UI5 Icon Explorer](httpsui5.sap.comtest-resourcessapmdemokiticonExplorerwebappindex.html#overviewSAP-icons) A handy tool to browse the SAP Fiori icon font
 [SAP Analytics Cloud Help](httpshelp.sap.comdoc00f68c2e08b941f081002fd3691d86a72020.1de-DEca67817bec1c4f6582126d5d9dab68bb.html#loioca67817bec1c4f6582126d5d9dab68bb__s_appearance) Instructions for loading custom fonts

## License

This repository licensed under the Apache Software License, v.2 except as noted otherwise in the [LICENSE](LICENSE) file.

Enjoy!











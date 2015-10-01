<properties pageTitle="Known Issues - NPM"
  description="This is an article on bower tutorial"
  services=""
  documentationCenter=""
  authors="kirupa" />
  <tags
     ms.service="na"
     ms.devlang="javascript"
     ms.topic="article"
     ms.tgt_pltfrm="mobile-multiple"
     ms.workload="na"
     ms.date="09/10/2015"
     ms.author="kirupac"/>

#**Known Issues - NPM**
**NPM Proxy Errors**

If NPM packages aren't installing properly, and you see an error that mentions bad characters in a request, the most likely cause is that there is a proxy/firewall interfering. To fix the issue, execute the following on the command prompt:

~~~~~~~~~~~~~
npm config set proxy http://proxydomain:port/
npm config set registry http://registry.npmjs.org/
~~~~~~~~~~~~~

**Note**: If you feel like you are seeing this error despite having configured the NPM proxy, it is possible that upgrading your Cordova version to 5.3.1 will fix the issue.
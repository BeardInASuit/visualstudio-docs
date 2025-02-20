---
title: Enable ClickOnce Security Settings | Microsoft Docs
description: Learn how the Publish wizard automatically enables code access security for ClickOnce applications to publish the application.
ms.custom: SEO-VS-2020
ms.date: 11/04/2016
ms.topic: how-to
dev_langs: 
  - VB
  - CSharp
  - C++
helpviewer_keywords: 
  - security [Visual Studio], ClickOnce applications
  - ClickOnce deployment, security settings
  - security settings, ClickOnce deployment
ms.assetid: 73cd3e9d-cd72-4ad2-8cae-94d6bb6b01e0
author: mikejo5000
ms.author: mikejo
manager: jmartens
ms.technology: vs-ide-deployment
ms.workload: 
  - multiple
---
# How to: Enable ClickOnce security settings

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Code access security for ClickOnce applications must be enabled in order to publish the application. This is done automatically when you publish an application using the Publish wizard.

 In some cases, enabling code access security can impact performance when building or debugging your application; in these cases, you may wish to temporarily disable the security settings.

 ClickOnce security settings can be enabled or disabled on the **Security** page of the **Project Designer**.

### To enable ClickOnce security settings

1. With a project selected in **Solution Explorer**, on the **Project** menu, click **Properties**.

2. Click the **Security** tab.

3. Select the **Enable ClickOnce Security Settings** check box.

     You can now customize the security settings for your application on the Security page.

    > [!NOTE]
    > This check box is automatically selected each time the application is published with the **Publish** wizard.

### To disable ClickOnce security settings

1. With a project selected in **Solution Explorer**, on the **Project** menu, click **Properties**.

2. Click the **Security** tab.

3. Clear the **Enable ClickOnce Security Settings** check box.

     Your application will be run with the full trust security settings; any settings on the **Security** page will be ignored.

    > [!NOTE]
    > Each time the application is published with the Publish wizard, this check box will be selected; you must clear it again after each successful publish.

## See also
- [Secure ClickOnce applications](../deployment/securing-clickonce-applications.md)
- [Code access security for ClickOnce applications](../deployment/code-access-security-for-clickonce-applications.md)

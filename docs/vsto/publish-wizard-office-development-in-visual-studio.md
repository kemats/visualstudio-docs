---
title: "Publish Wizard (Office Development in Visual Studio) | Microsoft Docs"
ms.custom: ""
ms.date: "02/02/2017"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "office-development"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "VST.ProjectProperties.PublishWizard"
  - "VST.PublishWizard.Publish.2007System"
dev_langs: 
  - "VB"
  - "CSharp"
helpviewer_keywords: 
  - "ClickOnce deployment [Office development in Visual Studio], Publish Wizard"
  - "deploying applications [Office development in Visual Studio], Publish Wizard"
  - "Office applications [Office development in Visual Studio], Publish Wizard"
  - "Publish Wizard, Office solutions"
ms.assetid: 793314b6-b6a6-4509-8f1c-dd9466cf5190
caps.latest.revision: 17
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
---
# Publish Wizard (Office Development in Visual Studio)
  Use the **Publish Wizard** to copy solution files to a specified location, create the manifest files, and create a Setup program.  
  
 To access this wizard, on the **Build** menu, choose **Publish** *SolutionName*. You can also access the **Publish Wizard** from **Solution Explorer**. Open the shortcut menu for the project node, and then choose **Publish**.  
  
 Each section below describes a page of the wizard.  
  
## Where do you want to publish the application?  
 **Specify the location to publish this application**  
 Required. The publish location is the directory where the **Publish Wizard** copies the solution files such as the manifests, assemblies, temporary certificate, and other files from the build. You must have write access to this directory.  
  
 Type the location as a disk path, file share, FTP site, or web site URL, or click the **Browse** button to browse for the location. The path can be in these formats:  
  
-   A relative or absolute path in standard Windows format, such as C:\Deploy\MyApplication or \MyApplication.  
  
-   A Universal Naming Convention (UNC) path, such as \\\ServerName\MyApplication\\.  
  
-   A URL of a web site, such as http://www.microsoft.com/MyApplication.  
  
 By default, the publishing location is *http://localhost/projectname/* if you have IIS installed, or the publish\ directory if you do not have IIS installed.  
  
> [!NOTE]  
>  There are more considerations if the target computer is running Windows Vista. You must be an administrator on the Windows Vista computer to use the local publish option. In addition, the default location is always the *publish\\* directory, regardless of whether you have IIS installed.  
  
## What is the default installation path on end user computers?  
 The installation path is optional. You can set the installation path later if you prefer. For details, see [How to: Change the Installation Path of an Office Solution](http://msdn.microsoft.com/en-us/d0eaa07b-2d72-4902-899f-2f9fb165b8fd).  
  
 The installation path is the directory from which the end user will install the customization. It is also the path that the solution will use to check for updates. The **Publish Wizard** does not deploy the solution to this location, unless the path is the same as the one you entered in the **Specify the location to publish this application** box on the previous page.  
  
 **From a Web site**  
 Specify the URL that end users will follow to install the solution.  
  
 **From a UNC path or file share**  
 Specify the UNC path that end users will follow to install the solution.  
  
 **From a CD-ROM or DVD-ROM**  
 This option does not require an installation path.  
  
 Visual Studio does not burn the CD or DVD. You must copy the output to a CD or DVD manually.  
  
## See Also  
 [Deploying an Office Solution by Using ClickOnce](../vsto/deploying-an-office-solution-by-using-clickonce.md)   
 [Publish Page, Project Designer &#40;Office Development in Visual Studio&#41;](../vsto/publish-page-project-designer-office-development-in-visual-studio.md)   
 [Deploying an Office Solution](../vsto/deploying-an-office-solution.md)  
  
  
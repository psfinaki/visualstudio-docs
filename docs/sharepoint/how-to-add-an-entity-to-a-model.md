---
title: "How to: Add an Entity to a Model | Microsoft Docs"
description: Add an entity to a model by adding an entity control from the Visual Studio Toolbox onto the Business Data Connectivity (BDC) designer.
ms.custom: SEO-VS-2020
ms.date: "02/02/2017"
ms.topic: how-to
f1_keywords:
  - "EntityTool"
dev_langs:
  - "VB"
  - "CSharp"
helpviewer_keywords:
  - "BDC [SharePoint development in Visual Studio], entity"
  - "Business Data Connectivity service [SharePoint development in Visual Studio], adding an entity"
  - "Business Data Connectivity service [SharePoint development in Visual Studio], entity"
  - "BDC [SharePoint development in Visual Studio], adding an entity"
author: John-Hart
ms.author: johnhart
manager: jmartens
ms.technology: sharepoint-development
ms.workload:
  - "office"
---
# How to: Add an entity to a model

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
  To create an entity, add an entity control from the Visual Studio **Toolbox** onto the Business Data Connectivity (BDC) designer.

### To add an entity to the model

1. Create a BDC project, or open an existing BDC project. For more information, see [Create a business data connectivity model](../sharepoint/creating-a-business-data-connectivity-model.md).

2. In the **Toolbox**, from the **BusinessDataCatalog** group, add an **Entity** control onto the designer.

     The new entity appears on the designer. Visual Studio adds an `<Entity>` element to the XML of the BDC model file in your project. For more information about the attributes of an Entity element, see [Entity](/previous-versions/office/developer/sharepoint-2010/ee558325(v=office.14)).

3. On the designer, open the shortcut menu for the entity, choose **Add**, and then choose **Identifier**.

     A new identifier appears on the entity.

    > [!NOTE]
    > You can change the name of the entity and the identifier in the **Properties** window.

4. Define the fields of the entity in a class. You can either add a new class to the project or use an existing class created by using other tools such as the Object Relational Designer (O/R Designer). The following example shows an entity class named Contact.

    ### [C#](#tab/csharp)
    :::code language="csharp" source="../sharepoint/codesnippet/CSharp/sp_bdc_entity_data_class/bdcmodel1/contact.cs" id="Snippet1":::

    ### [VB](#tab/vb)
    :::code language="vb" source="../sharepoint/codesnippet/VisualBasic/sp_bdc_entity_data_class/bdcmodel1/contact.vb" id="Snippet1":::
    ---

## See also
- [How to: Add a Creator method](../sharepoint/how-to-add-a-creator-method.md)
- [How to: Add a Deleter method](../sharepoint/how-to-add-a-deleter-method.md)
- [How to: Add an Updater method](../sharepoint/how-to-add-an-updater-method.md)
- [How to: Add a Finder method](../sharepoint/how-to-add-a-finder-method.md)
- [How to: Add a specific Finder method](../sharepoint/how-to-add-a-specific-finder-method.md)

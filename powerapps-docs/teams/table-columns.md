---
title: Work with Dataverse for Teams table columns | Microsoft Docs
description: Explains how to create and use Dataverse for Teams table columns.
author: NHelgren
ms.service: powerapps
ms.topic: conceptual
ms.custom: 
ms.date: 09/22/2020
ms.author: nhelgren
ms.reviewer: matp
---

# Work with table columns

With the exception of the Customer field, all field types in Dataverse are available in Dataverse for Teams as *columns*. This article covers the content you'll need for working with table columns in Dataverse for Teams.

Notice that the currency feature will always use the default currency for the country that was selected during Dataverse for Teams environment creation. This can't be changed, and additional transaction currencies or exchange rates can't be added. However, you can upgrade from Dataverse for Teams to Dataverse for full currency functionality.

For more information about the columns available, see these Dataverse articles:

- [Fields overview](../maker/data-platform/fields-overview.md)
- [Create and edit global option sets overview](../maker/data-platform/create-edit-global-option-sets.md)
- [Autonumber fields](../maker/data-platform/autonumber-fields.md)
- [Set managed properties for fields](../maker/data-platform/set-managed-properties-for-field.md)
- [Behavior and format of the Date and Time field](../maker/data-platform/behavior-format-date-time-field.md)

## Create a column

1. On the **Build** tab, select **See all**, and then expand **Tables**. 
2. Select the table you want to add a column to, and then select **Add column** on the command bar.
    > [!div class="mx-imgBorder"] 
    > ![Create a table column](media/create-table-column.png "Create a table column")

The rest of the process to add and manage columns is the same as in Dataverse, which is documented in these articles:
- [Create and edit fields for Dataverse using Power Apps portal](../maker/data-platform/create-edit-field-portal.md)
- [Manage custom fields in an entity](../maker/data-platform/data-platform-manage-fields.md)

## Choice columns

In Dataverse for Teams, choices can only be created as a column within a table. Creating choices is otherwise the same as creating an option set in Dataverse. More information: [Create an Option set](../maker/data-platform/custom-picklists.md)

## Calculated and rollup columns

The calculated columns and rollup columns that are available in Dataverse for Teams are equivalent to what's available in Dataverse. More information: [Define calculated fields to automate manual calculations](../maker/data-platform/define-calculated-fields.md) and [Define rollup fields that aggregate values](../maker/data-platform/define-rollup-fields.md)

### See also

[Create a table](create-table.md)

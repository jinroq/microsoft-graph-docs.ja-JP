---
author: daspek
ms.author: dspektor
title: renameAction リソースの種類
description: RenameAction オブジェクトは、アイテムの名前を変更したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bce040130d74b7977fc1f988a34edde674f9e0d4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970763"
---
# <a name="renameaction-resource-type"></a>renameAction リソースの種類

[**Itemactivity**] [ activity]に**renameaction**リソースが存在することは、アクティビティがアイテムの名前を変更したことを示します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[activity]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| oldName       | string | アイテムの変更前の名前。
| newName       | string | アイテムの新しい名前を指定します。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->

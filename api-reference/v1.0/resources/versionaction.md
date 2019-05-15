---
author: daspek
ms.author: dspektor
title: versionAction リソースの種類
description: VersionAction オブジェクトは、新しいアイテムバージョンが発生したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0d05ad93c59ba736dd90276fc5e3db6e05740344
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970753"
---
# <a name="versionaction-resource-type"></a>versionAction リソースの種類

[**Itemactivity**] [ activity]に**versionaction**リソースがある場合、アクティビティが新しいバージョンの作成を引き起こしたことを示します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[activity]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| newVersion    | string | このアクションによって作成された新しいバージョンの名前。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->

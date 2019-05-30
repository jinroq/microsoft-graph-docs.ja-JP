---
author: daspek
ms.author: dspektor
title: itemActivity リソースの種類
description: ItemActivity オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 98ae9e4881de18c94490469b10df43b2aaf58140
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536688"
---
# <a name="itemactivity-resource-type"></a>itemActivity リソースの種類

**Itemactivity**リソースは、アイテムまたはコンテナー内で行われたアクティビティに関する情報を提供します。
現在、SharePoint と OneDrive for Business でのみ使用できます。

ItemActivity 内で行われたアクションは、 [Itemactionset][]プロパティで詳細に説明されています。

>**注:****Itemactivity**は現在、SharePoint と OneDrive for business でのみ使用できます。

[itemActionSet]: itemactionset.md#properties

## <a name="properties"></a>プロパティ

| プロパティ | 型                    | 説明
|:---------|:------------------------|:----------------------------------------
| id       | string                  | アクティビティの一意識別子。 読み取り専用です。
| 接続   | [accessAction][]        | アイテムがアクセスされました。
| actor    | [identitySet][]         | アクションを実行したユーザーの識別情報。 読み取り専用です。
| activityDateTime    | DateTimeOffset | アクティビティがいつ発生したかについての詳細。 読み取り専用です。

[accessAction]: accessaction.md
[identitySet]: identityset.md

## <a name="relationships"></a>リレーションシップ

| リレーションシップ名 | 種類          | 説明
|:------------------|:--------------|:-----------------------------------------
| driveItem         | [driveItem][] | このアクティビティのターゲットとなった **driveItem** を表します。
| listItem          | [listItem][]  | このアクティビティのターゲットとなった **listItem** を表します。

[driveItem]: driveitem.md
[listItem]: listitem.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivity",
  "@type.aka": "oneDrive.activityEntity"
}-->

```json
{
  "id": "string (identifier)",
  "access": "microsoft.graph.accessAction",
  "actor": {"@odata.type": "microsoft.graph.identitySet"},
  "driveItem": {"@odata.type": "microsoft.graph.driveItem"},
  "listItem": {"@odata.type": "microsoft.graph.listItem"},
  "activityDateTime": {"@odata.type": "String (timestamp)"}
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActivity object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActivity",
  "suppressions": []
}
-->

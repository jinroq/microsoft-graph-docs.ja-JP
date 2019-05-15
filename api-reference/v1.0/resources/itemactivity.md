---
author: daspek
ms.author: dspektor
title: itemActivity リソースの種類
description: ItemActivity オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c05493ddeb8e007da6ba8b7508369b4d013e672
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970757"
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
| ID       | string                  | アクティビティの一意識別子。 値の取得のみ可能です。
| 接続   | [accessAction][]        | アイテムがアクセスされました。
| actor    | [identitySet][]         | アクションを実行したユーザーの識別情報。 値の取得のみ可能です。
| activityDateTime    | DateTimeOffset | アクティビティがいつ発生したかについての詳細。 読み取り専用です。

[accessAction]: accessAction.md
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

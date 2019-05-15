---
author: daspek
ms.author: dspektor
title: itemActivityTimeSet リソースの種類
description: ItemActionSet オブジェクトは、アイテムに対して行われたアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4ef0b56471afe78b13edc2f6efb25941c9a749df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970776"
---
# <a name="itemactivitytimeset-resource-type"></a>itemActivityTimeSet リソースの種類

**Itemactivitytimeset**リソースは、アイテムの[アクティビティ][ activity]が実行された日時に関する情報を提供します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[activity]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名    | 種類           | 説明
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | アクティビティの発生が確認されたとき。
| recordedDateTime | DateTimeOffset | アクティビティの確認がサービスに記録されたとき。

**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。
ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。
後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "keyProperty": "id",
  "@type": "microsoft.graph.itemActivityTimeSet",
  "@type.aka": "oneDrive.times",
  "@property.aka": "observedDateTime=observedTime recordedDateTime=recordedTime"
}-->

```json
{
  "observedDateTime": "String (timestamp)",
  "recordedDateTime": "String (timestamp)"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/itemActionSet",
  "suppressions": []
}
-->

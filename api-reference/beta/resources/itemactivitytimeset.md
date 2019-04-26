---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
ms.openlocfilehash: 999949f788c215a1e0645577a14b540586108926
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345417"
---
# <a name="itemactivitytimeset-resource-type"></a>ItemActivityTimeSet リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**ItemActivityTimeSet** リソースは、アイテムに対する[アクティビティ][activity]がいつ発生したかに関する情報を提供します。

[activity]: itemactivity.md

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

## <a name="properties"></a>プロパティ

| プロパティ名    | 種類           | 説明
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | アクティビティの発生が確認されたとき。
| recordedDateTime | DateTimeOffset | アクティビティの確認がサービスに記録されたとき。

**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。
ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。
後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet",
  "suppressions": []
}
-->

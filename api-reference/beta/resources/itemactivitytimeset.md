---
author: daspek
description: ItemActivityTimeSet リソースは、アイテムに対するアクティビティがいつ発生したかに関する情報を提供します。
ms.date: 09/14/2017
title: ItemActivityTimeSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c81bf7885ee1466e293236a987e90e21323daefd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010092"
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

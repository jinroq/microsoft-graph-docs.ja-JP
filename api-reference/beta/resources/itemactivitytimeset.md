---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ItemActivityTimeSet
ms.openlocfilehash: 7a8852af9fc9c99f69b8d61f53037be91f35b31e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074098"
---
# <a name="itemactivitytimeset-resource-type"></a>ItemActivityTimeSet リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

| プロパティ名    | 型           | 説明
|:-----------------|:---------------|:-----------------------------------------
| observedDateTime | DateTimeOffset | アクティビティの発生が確認されたとき。
| recordedDateTime | DateTimeOffset | アクティビティの確認がサービスに記録されたとき。

**確認された時間**と**記録された時間**の差は、オフライン コラボレーションのシナリオにとって特に重要です。
ユーザーがオフラインでファイルにコメントする場合、コメントした時刻は **observedDateTime** に設定されます。
後でユーザーがクラウドに再接続し、変更がアップロードされるとき、その時刻は **recordedDateTime** に設定されます。

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!-- {
  "type": "#page.annotation",
  "description": "The ItemActionSet object provides information about an activity that took place on an item.",
  "keywords": "activities,activity,action",
  "section": "documentation",
  "tocPath": "Resources/ItemActionSet"
} -->

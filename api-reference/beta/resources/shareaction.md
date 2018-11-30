---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: ShareAction
ms.openlocfilehash: c9f06c7a4a6351b8a6554c944c0efe9af379e030
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070650"
---
# <a name="shareaction-resource-type"></a>ShareAction リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**ShareAction** リソースは、アイテムを共有した[アクティビティ][activity]に関する情報を提供します。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.shareAction"
}-->

```json
{
  "recipients": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 型                       | 説明
|:--------------|:---------------------------|:-----------------------------
| recipients    | [identitySet][] コレクション | このアクションでアイテムが共有された相手の ID。

[identitySet]: identityset.md

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!-- {
  "type": "#page.annotation",
  "description": "The ShareAction object provides information about who an item was shared to in a share action.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/ShareAction"
} -->

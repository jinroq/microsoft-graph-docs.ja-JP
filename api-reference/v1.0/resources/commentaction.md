---
author: daspek
ms.author: dspektor
title: コメントアクションリソースの種類
description: Comment アクションオブジェクトは、アイテムに対して行われたコメントについての情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 12e6cd68d5809b8e4c1765234eeb77b40b30a78e
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970749"
---
# <a name="commentaction-resource-type"></a>コメントアクションリソースの種類

**Comment アクション**リソースは、アイテムに対して行われたコメント[アクティビティ][]に関する情報を提供します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[アクティビティ]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名    | 種類                       | 説明
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。
| parentAuthor     | [identitySet][]            | コメント スレッドを開始したユーザーの ID。
| participants     | [identitySet][] コレクション | 該当のコメント スレッドに参加しているユーザーの ID。

[identitySet]: identityset.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->

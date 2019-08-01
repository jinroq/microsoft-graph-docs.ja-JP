---
author: daspek
ms.author: dspektor
title: コメントアクションリソースの種類
description: Comment アクションオブジェクトは、アイテムに対して行われたコメントについての情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 72502e466ff90ec0a299eb993346968c9038e2d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029681"
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

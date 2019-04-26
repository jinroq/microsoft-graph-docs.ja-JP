---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: c472a0b1b992c91b60174859e4900ffcee04c007
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341482"
---
# <a name="commentaction-resource-type"></a>CommentAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**CommentAction**リソースは、アイテムに対して行われたコメント [アクティビティ][]に関する情報を提供します。

[アクティビティ]: itemactivity.md

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

## <a name="properties"></a>プロパティ

| プロパティ名    | 種類                       | 説明
|:-----------------|:---------------------------|:-----------------------------
| isReply          | boolean                    | true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。
| parentAuthor     | [identitySet][]            | コメント スレッドを開始したユーザーの ID。
| participants     | [identitySet][] コレクション | 該当のコメント スレッドに参加しているユーザーの ID。

[identitySet]: identityset.md

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->

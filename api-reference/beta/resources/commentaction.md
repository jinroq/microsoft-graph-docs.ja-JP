---
author: daspek
description: CommentActionリソースは、アイテムに対して行われたコメント アクティビティに関する情報を提供します。
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7782c6e4dd30b503a9be88737ef6bd2dbad109b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973259"
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

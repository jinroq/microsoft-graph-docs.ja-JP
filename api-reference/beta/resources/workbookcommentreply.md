---
title: workbookCommentReply リソースの種類
description: WorkbookCommentReply リソースの種類の定義
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0a4dfc215eec435c67f1259a85e899db4dfb2b63
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775903"
---
# <a name="workbookcommentreply-resource-type"></a>workbookCommentReply リソースの種類

Excel コメントへの返信を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リスト workbookCommentReplies](../api/workbookcomment-list-replies.md) | [workbookCommentReply](workbookcommentreply.md)コレクション | Workbookcommentreply オブジェクトのリストを取得します。 |
| [WorkbookCommentReply を取得する](../api/workbookcommentreply-get.md) | [workbookCommentReply](workbookcommentreply.md) | WorkbookCommentReply オブジェクトのプロパティとリレーションシップを読み取ります。 |
| [WorkbookCommentReply を作成する](../api/workbookcomment-post-replies.md) | [workbookCommentReply](workbookcommentreply.md) | 新しい workbookCommentReply を作成します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|content|String|返信されたコメントの内容。|
|contentType|String|返信されたコメントの種類を示します。|
|id|文字列|コメント ID を表します。 読み取り専用です。|

## <a name="relationships"></a>関係

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookCommentReply",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "content": "String",
  "contentType": "String",
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookCommentReply resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

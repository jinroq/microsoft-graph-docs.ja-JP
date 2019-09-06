---
title: workbookComment リソースの種類
description: ブック内のコメントを表します。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a7a3427512962bd38c90faa710c501380e353f22
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775896"
---
# <a name="workbookcomment-resource-type"></a>workbookComment リソースの種類

ブック内のコメントを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リスト workbookComments](../api/workbook-list-comments.md) | [workbookComment](workbookComment.md)コレクション | **WorkbookComment**オブジェクトのコレクションを取得します。 |
| [WorkbookComment を取得する](../api/workbookcomment-get.md) | [workbookComment](workbookcomment.md) | **WorkbookComment**オブジェクトのプロパティとリレーションシップを読み取ります。 |


## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|content|String|コメントの内容。|
|contentType|String|コメントの種類を示します。|
|id|文字列| コメント ID を表します。 読み取り専用です。|

## <a name="relationships"></a>関係

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|replies|[workbookCommentReply](workbookcommentreply.md)コレクション| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookComment",
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
  "description": "workbookComment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

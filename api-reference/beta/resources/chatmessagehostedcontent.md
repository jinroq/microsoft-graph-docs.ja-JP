---
title: chatMessageHostedContent リソースの種類
description: チャットメッセージでホストされているコンテンツ
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2787138819160a25d72fb9ed273950eee326399c
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720951"
---
# <a name="chatmessagehostedcontent-resource-type"></a>chatMessageHostedContent リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

画像やコードスニペットなど、チャットメッセージでホストされているコンテンツを表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [ChatMessageHostedContent を取得する](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | **ChatMessageHostedContent**オブジェクトのプロパティとリレーションシップを読み取ります。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|id|String| 読み取り専用です。|

## <a name="relationships"></a>関係

なし。

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
title: chatThread リソース型
description: ChatThread は、Microsoft Teams における chatMessages のコレクションです。
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521342"
---
# <a name="chatthread-resource-type"></a>chatThread リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

chatThread は、Microsoft Teams における [chatMessages](chatmessage.md) のコレクションです。

> 現在のところ、ChatThreads は[チャネル内で作成](../api/channel-post-chatthreads.md)できます。  API の今後のリリースでは、既存の chatThreads の読み取りに加えて、チームやチャネルの範囲外のユーザー間での直接チャットの読み取り/書き込みをサポートします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Create thread](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |最初のメッセージを指定して、指定したチャネルで新しいスレッドを開始します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Null 許容型。|
|chatMessages|[chatMessage](chatmessage.md) コレクション| Null 許容型。|

> 現在、これらの関係は暗黙的に存在しますが、読み取り/書き込みはできません。  将来的に、ベータ版の API リリースでこの機能がサポートされます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

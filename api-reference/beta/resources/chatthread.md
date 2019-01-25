---
title: chatThread リソース型
description: ChatThread は、Microsoft Teams における chatMessages のコレクションです。
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399606"
---
# <a name="chatthread-resource-type"></a>chatThread リソース型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

ChatThread は、Microsoft Teams における [chatMessages](chatmessage.md) のコレクションです。

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
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

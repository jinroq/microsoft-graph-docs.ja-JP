---
title: chatThread リソースの種類
description: ChatThread は、マイクロソフトのチームでの chatMessages のコレクションです。
localization_priority: Priority
ms.openlocfilehash: 5060d7ea846f5aedec5551aaf247642a36f73c1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833244"
---
# <a name="chatthread-resource-type"></a>chatThread リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ChatThread は、マイクロソフトのチームでは、 [chatMessages](chatmessage.md)のコレクションです。

> 現時点では、chatThreads、[チャネルで作成](../api/channel-post-chatthreads.md)します。  API の将来のリリースでは、チームまたはチャネルの範囲外にいるユーザーの間で直接チャットを読み取り/書き込みと同様に、既存の chatThreads の読み取りをサポートします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[スレッドを作成する](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |指定のチャネルでは、最初のメッセージを提供する新しいスレッドを開始します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|ID|String| 読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| Null 許容型。|
|chatMessages|[chatMessage](chatmessage.md)コレクション| Null 許容型。|

> 現在これらの関係、暗黙的に存在が、ことはできませんを読み取ったり書き込んだりします。  今後 API のベータ版のリリースは、これをサポートします。

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
  "id": "string (identifier)",
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

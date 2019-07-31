---
title: chatMessageHostedImage リソースの種類
description: ChatMessage 内のホストされているイメージを表します。
localization_priority: Normal
author: clearab
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e217234b8ea6c6510b85af1bf1002e589e4366e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974004"
---
# <a name="chatmessagehostedimage-resource-type"></a>chatMessageHostedImage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Chatmessage](../resources/chatmessage.md)内のホストされているイメージを表します。

ホストされた画像は、メッセージの本文に表示されるイメージです\<。 img> タグの内容は、で`https://graph.microsoft.com`始まる src 属性を使用し**ます。**

メッセージ内の画像がホストされているわけではないため、Microsoft Teams も (img src 属性がパブリック web サイトをポイントする) パブリック画像をサポートしています。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[ChatMessage 内の chatMessageHostedImages を一覧表示する](../api/chatmessagehostedimage-list-hostedimages.md) | [Chatmessagehostedimage](chatmessagehostedimage.md)コレクション | **Chatmessage**でホストされているすべての画像のリスト。|
|[ChatMessageHostedImage を取得する](../api/chatmessagehostedimage-get.md) | [chatMessageHostedImage](chatmessagehostedimage.md) | 1つのホストイメージを取得します。|
|[chatMessageHostedImage: getBytes](../api/chatmessagehostedimage-getbytes.md) | コンテンツタイプ: image/jpeg | ホストされているイメージの生バイトを取得します。|

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String| 読み取り専用です。 メッセージの一意の ID。|
|URL| string | 画像コンテンツを取得する url。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

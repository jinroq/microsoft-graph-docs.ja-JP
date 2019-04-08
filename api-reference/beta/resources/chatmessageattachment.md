---
title: chatmessageattachment リソースの種類
description: チャットメッセージエンティティへの添付ファイルを表します。
localization_priority: Normal
ms.openlocfilehash: 6445da35f86e5e046a07797e1f28e9dfaec8a863
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481399"
---
# <a name="chatmessageattachment-resource-type"></a>chatmessageattachment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チャットメッセージエンティティへの添付ファイルを表します。

型`chatMessageAttachment`のエンティティは、 [chatmessage](chatmessage.md)エンティティの一部として、 [Get channel messages](../api/channel-list-messages.md) API の一部として返されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string| 読み取り専用です。 添付ファイルの一意の id です。|
|contentType| string | コンテンツの添付ファイルのメディアの種類。 次の値を指定できます。 <br><ul><li>参照: Attachment は、別のファイルへのリンクです。 contenturl に、オブジェクトへのリンクを設定します。<br></li><li>ファイル: Raw ファイル添付ファイル。 contenturl フィールドに、data: 形式のファイルの base64 エンコードを設定します。<br></li><li>画像/: 画像の種類 (画像/png、画像/jpeg、画像/gif) を指定した画像の種類。 contenturl フィールドに、data: 形式のファイルの base64 エンコードを設定します。<br></li><li>ビデオ/: 形式が指定されたビデオの種類。 Ex: video/mp4。 contenturl フィールドに、data: 形式のファイルの base64 エンコードを設定します。<br></li><li>audio/: 指定された形式のオーディオタイプ。 Ex: 音声/wmw contenturl フィールドに、data: 形式のファイルの base64 エンコードを設定します。<br></li><li>アプリケーション/カードの種類: カードの種類がリッチカードの添付ファイルで、使用する正確なカード形式を指定します。 カードの json 形式でコンテンツを設定します。 カード型でサポートされている値は次のとおりです。<br><ul><li>application/vnd: テキスト、音声、画像、ボタン、および入力フィールドの任意の組み合わせを含むことができるリッチカード。 content プロパティを、AdaptiveCard オブジェクトに設定します。</li><li>アプリケーション/vnd。アニメーション: アニメーションを再生するリッチカード。 コンテンツプロパティを、アニメーションの cardobject に設定します。</li><li>application/vnd audio: オーディオファイルを再生するリッチカード。 content プロパティを AudioCard オブジェクトに設定します。</li><li>application/vnd ビデオ: ビデオを再生するリッチカード。 content プロパティを VideoCard オブジェクトに設定します。</li><li>アプリケーション/vnd。ヒーロー: 英雄カード。 content プロパティを HeroCard オブジェクトに設定します。</li><li>application/vnd-サムネイルカード: サムネイルカード。 content プロパティを ThumbnailCard オブジェクトに設定します。</li><li>アプリケーション/vnd。領収書: 領収書カード。 content プロパティを ReceiptCard オブジェクトに設定します。</li><li>アプリケーション/vnd: ユーザーがサインインカードをサインインします。 content プロパティを SignInCard オブジェクトに設定します。</ul></ul>|
|contentUrl|文字列|添付ファイルのコンテンツの URL。 サポートされているプロトコル: http、https、ファイル、およびデータ。|
|content|string|添付ファイルの内容。 添付ファイルがリッチカードの場合は、プロパティをリッチカードオブジェクトに設定します。 このプロパティと contenturl は相互に排他的です。|
|name|string|添付ファイルの名前を指定します。|
|thumbnailUrl| string |別の小さな形式のコンテンツまたは contenturl を使用してサポートされている場合に、チャネルが使用できるサムネイルイメージの URL。 たとえば、contentType を application/word に設定して、contenturl を word 文書の場所に設定した場合、ドキュメントを表すサムネイルイメージを含めることができます。 チャネルは、ドキュメントの代わりにサムネイルイメージを表示することができます。 ユーザーが画像をクリックすると、チャネルはドキュメントを開きます。|

## <a name="json-representation"></a>JSON 表記
 リソースの JSON 表記を次に示します

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessageattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

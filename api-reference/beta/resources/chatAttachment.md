---
title: chatMessageAttachment リソースの種類
description: チャット メッセージのエンティティの添付ファイルを表します。
localization_priority: Normal
ms.openlocfilehash: 12682ee090a2dc7976db46629cd26df9e5b1595e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640918"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

チャット メッセージのエンティティの添付ファイルを表します。

エンティティの種類の`chatMessageAttachment` [chatMessage](chatmessage.md)エンティティの一部として、[チャネルのメッセージを取得する](../api/channel-list-messages.md)API の一部として返されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|string| 読み取り専用です。 添付ファイルの一意の id です。|
|contentType| string | コンテンツの添付ファイルのメディア ・ タイプ。 次の値を持つ、ことができます。 <br><ul><li>参照: 添付ファイルは、別のファイルへのリンクです。 オブジェクトへのリンクに contentURL を設定します。<br></li><li>ファイル: Raw ファイルの添付ファイルです。 データ内のファイルの base64 エンコードを使用して contenturl フィールドを設定します。 形式です。<br></li><li>イメージ/: ex 指定したイメージの種類のイメージの種類: イメージまたは png、jpeg のイメージと、イメージまたは gif です。 データ内のファイルの base64 エンコードを使用して contentUrl フィールドを設定します。 形式です。<br></li><li>ビデオと: 指定された形式でビデオの種類です。 Ex: ビデオと mp4 です。 データ内のファイルの base64 エンコードを使用して contentUrl フィールドを設定します。 形式です。<br></li><li>オーディオ/: 指定された形式でのオーディオの種類です。 Ex: オーディオ/wmw。 データ内のファイルの base64 エンコードを使用して contentUrl フィールドを設定します。 形式です。<br></li><li>アプリケーションとカードの種類: カードを使用するカードの正確な形式を指定するカードの種類の添付ファイルの種類の豊富な。 カードの json 形式のコンテンツを設定します。 カードの種類でサポートされる値は次のとおりです。<br><ul><li>application/vnd.microsoft.card.adaptive: テキスト、音声、画像、ボタン、および入力フィールドの任意の組み合わせを含めることができる豊富なカードです。 AdaptiveCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.animation: アニメーションを再生する豊富なカードです。 AnimationCardobject に、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.audio: オーディオ ファイルを再生する豊富なカードです。 AudioCard オブジェクトに、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.video: ビデオを再生する豊富なカードです。 使いのビデオカードのオブジェクトをコンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.hero: 英雄カードです。 HeroCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.thumbnail: サムネイルのカードです。 ThumbnailCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.com.card.receipt: レシートのカードです。 ReceiptCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.com.card.signin: ユーザーのサインインのカードです。 SignInCard オブジェクトには、コンテンツのプロパティを設定します。</ul></ul>|
|contentUrl|文字列|添付ファイルのコンテンツの URL です。 サポートされているプロトコル: http、https、ファイルおよびデータ。|
|content|string|添付ファイルの内容です。 添付ファイルが豊富なカードの場合は、豊富なカードのオブジェクトにプロパティを設定します。 このプロパティと contentUrl は、相互に排他的です。|
|name|string|添付ファイルの名前です。|
|thumbnailUrl| string |URL、サムネイル イメージをコンテンツまたは contentUrl の小さい、代替フォームを使用してサポートしている場合、チャネルを使用できます。 たとえばかどうか、したアプリケーション、word にコンテンツ タイプを設定して Word 文書の場所に contentUrl を設定、する可能性がありますが含まれますドキュメントを表すサムネイル画像にはです。 チャネルは、ドキュメントではなく、サムネイル イメージを表示できます。 ユーザーは、画像をクリックすると、チャネルがドキュメントを開きます。|

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
    "Error: /api-reference/beta/resources/chatAttachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

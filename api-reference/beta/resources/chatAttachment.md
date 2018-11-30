---
title: chatMessageAttachment リソースの種類
description: チャット メッセージのエンティティの添付ファイルを表します。
ms.openlocfilehash: 65390caa417b6130a84fada2a089b31125da288a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067816"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

チャット メッセージのエンティティの添付ファイルを表します。

エンティティの種類の`chatMessageAttachment` [chatMessage](chatmessage.md)エンティティの一部として、[チャネルのメッセージを取得する](../api/channel-list-messages.md)API の一部として返されます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ID|文字列| 読み取り専用です。 添付ファイルの一意の id|
|contentType| 文字列 | コンテンツの添付ファイルのメディア ・ タイプ。 次の値を持つ、ことができます。 <br><ul><li>参照: 添付ファイルは、別のファイルへのリンクです。 オブジェクトへのリンクに contentURL を設定します。<br></li><li>ファイル: Raw ファイルの添付ファイルです。 データ内のファイルの base64 エンコードを使用して contenturl フィールドを設定します書式設定。<br></li><li>イメージ/: ex 指定したイメージの種類のイメージの種類: イメージまたは png、jpeg のイメージと、イメージまたは gif です。 データ内のファイルの base64 エンコードを使用して contentUrl フィールドを設定します書式設定。<br></li><li>ビデオと: 指定された形式でビデオの種類です。 Ex: ビデオと mp4 です。 データ内のファイルの base64 エンコードを使用して contentUrl フィールドを設定します書式設定。<br></li><li>オーディオ/: 指定された形式でのオーディオの種類です。 Ex: オーディオ/wmw。 データ内のファイルの base64 エンコードを使用して contentUrl フィールドを設定します書式設定。<br></li><li>アプリケーションとカードの種類: カードを使用するカードの正確な形式を指定するカードの種類の添付ファイルの種類の豊富な。 カードの json 形式のコンテンツを設定します。 カードの種類でサポートされる値は次のとおりです。<br><ul><li>application/vnd.microsoft.card.adaptive: テキスト、音声、画像、ボタン、および入力フィールドの任意の組み合わせを含めることができる豊富なカードです。 AdaptiveCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.animation: アニメーションを再生する豊富なカードです。 AnimationCardobject に、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.audio: オーディオ ファイルを再生する豊富なカードです。 AudioCard オブジェクトに、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.video: ビデオを再生する豊富なカードです。 使いのビデオカードのオブジェクトをコンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.hero: 英雄カードです。 HeroCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.card.thumbnail: サムネイルのカードです。 ThumbnailCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.com.card.receipt: レシートのカードです。 ReceiptCard オブジェクトには、コンテンツのプロパティを設定します。</li><li>application/vnd.microsoft.com.card.signin: ユーザーのサインインのカードです。 SignInCard オブジェクトには、コンテンツのプロパティを設定します。</ul></ul>|
|contentUrl|文字列|添付ファイルのコンテンツの URL です。 サポートされているプロトコル: http、https、ファイルおよびデータ|
|content|文字列|添付ファイルの内容です。 添付ファイルが豊富なカードの場合は、豊富なカードのオブジェクトにプロパティを設定します。 このプロパティと contentUrl は相互に排他的です|
|name|文字列|添付ファイルの名前|
|thumbnailUrl| 文字列 |URL、サムネイル イメージをコンテンツまたは contentUrl の小さい、代替フォームを使用してサポートしている場合、チャネルを使用できます。 たとえばかどうか、したアプリケーション、word にコンテンツ タイプを設定して Word 文書の場所に contentUrl を設定、する可能性がありますが含まれますドキュメントを表すサムネイル画像にはです。 チャネルは、ドキュメントではなく、サムネイル イメージを表示できます。 ユーザーは、画像をクリックすると、チャネルがドキュメントを開きます。|

## <a name="json-representation"></a>JSON 表記
 次は、JSON 形式のリソース

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
<!-- {
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
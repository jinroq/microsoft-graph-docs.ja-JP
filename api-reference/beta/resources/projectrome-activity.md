---
title: アクティビティリソースの種類
description: アプリ内の1つのアクティビティを表します。たとえば、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなどがあります。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 4ae3fb47961140a784a1fa15fc606fd8967be96b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344019"
---
# <a name="activity-resource-type"></a>アクティビティリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリ内の1つのアクティビティを表します。たとえば、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなどがあります。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す[履歴項目](projectrome-historyitem.md)として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。

Microsoft Graph のアクティビティを使用すると、ユーザーが複数のデバイスでアプリで実行していた操作に戻れるようにすることができます。 アプリによって作成されるアクティビティは、すべてのユーザーのデバイスに表示され、アプリ内の特定のコンテンツへの詳細なリンクとしてユーザーに公開されます。 アプリ内の特定のコンテンツを、Windows で紹介されている送信先として表現し、Cortana 通知を介して iOS および Android デバイスでアクセスすることができます。

すべてのアプリは異なるため、アプリケーション内のアクションを Cortana とタイムラインで表示されるユーザーアクティビティにマップするための最善の方法を理解しておく必要があります。 たとえば、ゲームは各キャンペーンに対してアクティビティを作成し、ドキュメント作成アプリは固有のドキュメントごとにアクティビティを作成し、基幹業務アプリは各ワークフローのアクティビティを作成する場合があります。

ユーザーのアクティビティは、Cortana および Windows タイムラインのユーザーエクスペリエンスで紹介されています。これは、ユーザーが過去に作業したコンテンツに戻れるようにすることによって、ユーザーの生産性と効率を向上させることに重点を置いています。

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[アクティビティを作成または置換する](../api/projectrome-put-activity.md) | [アクティビティ](projectrome-activity.md) |既存のアクティビティ (upsert) を作成または置換します。 appactivityid は url セーフである必要があります (RFC 2396 の予約されていない文字を除くすべての文字を16進表記に変換する必要があります) が、元の appactivityid を url セーフにする必要はありません。 |
|[アクティビティを削除する](../api/projectrome-delete-activity.md) | No Content | そのユーザーの指定したアクティビティをアプリから削除します。|
|[アクティビティを取得する](../api/projectrome-get-activities.md) | [アクティビティ](projectrome-activity.md)のコレクション | 特定のユーザーのアプリのアクティビティを取得します。|
|[最近のアクティビティを取得する](../api/projectrome-get-recent-activities.md) | [アクティビティ](projectrome-activity.md)のコレクション | 指定されたユーザーのアプリの最新のアクティビティを取得し、最後に作成または更新された[履歴アイテム](projectrome-historyitem.md)に基づいて並べ替えます。|

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|usertimezone | String | 省略可能。 アクティビティを生成するために使用されたユーザーのデバイスがアクティビティの作成時にあるタイムゾーン。クロスプラットフォーム表現をサポートするために olson id として提供される値。|
|createdDateTime | DateTimeOffset | サーバーによって設定されます。 サーバー上でオブジェクトが作成された日時 (UTC)。 |
|lastModifiedDateTime | DateTimeOffset | サーバーによって設定されます。 サーバー上のオブジェクトが変更された日時 (UTC)。 |
|id | String | サーバーによって生成された ID。 URL アドレス指定に使用されます。|
|appactivityid | String | 必須。 発信者によって提供される、またはその後に不変である、アプリのコンテキスト内の一意のアクティビティ ID。|
|activitysourcehost | String | 必須。 アプリのクロスプラットフォーム id マッピングを表すドメインの URL。 マッピングは、ドメインでホストされている JSON ファイルとして、または Windows デベロッパーセンターから構成可能な JSON ファイルのいずれかとして格納されます。 JSON ファイルは、クロスプラットフォームアプリ識別子と呼ばれ、トップレベルドメインまたはサブドメインを含む HTTPS ドメインのルートでホストされます。 例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。 クロスプラットフォームのアプリ id ごとに一意のファイルとドメイン (またはサブドメイン) が必要です。 たとえば、Word と PowerPoint では、別のファイルとドメインが必要になります。|
|appDisplayName | String | 省略可能。 アプリがユーザーのローカルデバイスにインストールされていない場合に使用するアクティビティの生成に使用するアプリの短いテキストの説明。|
|activationUrl | String | 必須。 appId で表される最高のネイティブの操作でアクティビティを開始するために使用される URL。 ネイティブアプリが存在しない場合は、web ベースのアプリを起動する可能性があります。|
|fallbackurl | String | 省略可能。 web ベースのアプリでアクティビティを起動するために使用される URL (可能な場合)。|
|contentUrl | String | 省略可能。 ネイティブまたは web ベースのアプリの使用状況 (RSS フィード内のアイテムへのポインターなど) の外部でコンテンツをレンダリングできる場合に使用します。|
|visualelements| [visualinfo](../resources/projectrome-visualinfo.md) | 必須です。 UX でアクティビティをレンダリングするための情報を含むオブジェクト。|
|contentinfo | 型指定のない JSON オブジェクト | 省略可能。 [schema.org](https://schema.org)構文に従ったコンテンツの、データのカスタム部分。|
|expirationDateTime | DateTimeOffset | サーバーによって設定されます。 サーバー上のオブジェクトの有効期限が切れたときの日時。|
|status | string | サーバーによって設定されます。 有効なオブジェクトを識別するために使用される状態コード。 値: アクティブ、更新済み、削除済み、無視。|

## <a name="relationships"></a>リレーションシップ

|リレーションシップ | 型 | 説明|
|:------------|:-----|:-----------|
|historyItems| [履歴アイテム](../resources/projectrome-historyitem.md)のコレクション | 省略可能。 NavigationProperty/コンテインメント;アクティビティの履歴アイテムへのナビゲーションプロパティ。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "appDisplayName",
    "fallbackUrl",
    "contentUrl",
    "contentInfo",
    "visualElements",
    "historyItems"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activity"
}-->

```json
{
    "appActivityId": "String",
    "activitySourceHost": "String (host name/domain/URL)",
    "userTimezone": "String",
    "appDisplayName": "String",
    "activationUrl": "String (URL)",
    "contentUrl": "String (URL)",
    "fallbackUrl": "String (URL)",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "expirationDateTime": "DateTimeOffset",
    "id": "String",
    "status": "string",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

---
title: アクティビティのリソースの種類
description: -テレビ番組、ドキュメント、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
ms.openlocfilehash: 2c619cf2ad1707a8efa9d363344ccce93d92bb10
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070608"
---
# <a name="activity-resource-type"></a>アクティビティのリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

-テレビ番組、ドキュメント、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示します、[履歴項目](projectrome-historyitem.md)として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。

何のアプリケーションでは、複数のデバイスを取得するのにユーザーを有効にするのに Microsoft Graph でのアクティビティを使用できます。 アプリを作成する活動は、すべてのユーザーのデバイスに表示され、アプリ内で特定のコンテンツへの高度なリンクとしてユーザーに公開されます。 Cortana の通知によってあっにアクセスし、Windows では、紹介先として、アプリケーション内で特定のコンテンツを表現できます。

すべてのアプリケーションが異なるためにです Cortana およびタイムラインに表示されるユーザー ・ アクティビティをアプリケーション内で操作をマップする最善の方法を理解します。 などのゲームは、各キャンペーンの活動を作成可能性があります、文書作成アプリケーションはそれぞれ固有のドキュメントのアクティビティを作成可能性があり、基幹業務アプリケーションは、各ワークフローのアクティビティを作成可能性があります。

Cortana およびタイムラインの Windows ユーザー エクスペリエンスは、ユーザーの生産性と効率性を増やすことにより、過去に働いているコンテンツに戻ることに重点を置くに、ユーザーの作業中です。

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[活動の作成または](../api/projectrome-put-activity.md) | [アクティビティ](projectrome-activity.md) |作成または既存の活動 (アップサート) が置き換えられます。 AppActivityId は URL セーフ (RFC 2396 の予約文字は、16 進表現に変換する必要がありますを除くすべての文字) である必要がありますが、元の appActivityId は、URL セーフである必要はありません。 |
|[アクティビティを削除する](../api/projectrome-delete-activity.md) | 内容なし | アプリからそのユーザーの指定したアクティビティを削除します。|
|[アクティビティを取得します。](../api/projectrome-get-activities.md) | [活動](projectrome-activity.md)のコレクション | アプリが特定のユーザーのアクティビティを取得します。|
|[最近のアクティビティを取得する](../api/projectrome-get-recent-activities.md) | [活動](projectrome-activity.md)のコレクション | アプリが並べ替えられ、最も最近作成または更新された[historyItems](projectrome-historyitem.md)に基づいて、特定のユーザーの最新のアクティビティを取得します。|

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|userTimezone | String | 省略可能。 活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンクロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。|
|createdDateTime | DateTimeOffset | サーバーで設定します。 サーバー上にオブジェクトが作成されたときの utc 日時。 |
|lastModifiedDateTime | DateTimeOffset | サーバーで設定します。 サーバー上にオブジェクトが変更されたときの utc 日時。 |
|id | String | サーバーによって生成される ID が URL に対応するために使用します。|
|appActivityId | String | 必須。 呼び出し元によって、不変をその後提供された - アプリケーションのコンテキストで一意のアクティビティ ID です。|
|activitySourceHost | String | 必須。 アプリケーションのクロスプラット フォームの id のマッピングを表すドメインの URL です。 マッピングは、ドメインでホストされている JSON ファイルとして、ストアドや Windows デベロッパー センターを使用して構成できます。 JSON ファイルは、クロス プラットフォーム アプリケーション識別子の名前はまたはトップ レベルのドメイン レベルのいずれか、"HTTPS"ドメインのルートでホストされていますとサブのドメインが含まれます。 例: https://contoso.com または https://myapp.contoso.com。しかし、https://myapp.contoso.com/somepath は無効です。 クロスプラット フォームのアプリケーション id ごと、一意のファイルおよびドメイン (またはサブドメイン) をすることが必要です。 たとえば、PowerPoint と Word の別のファイルとドメインが必要です。|
|appDisplayName | String | 省略可能。 アプリケーションがユーザーのローカル デバイスにインストールされていない場合の場合に使用するための活動を生成するために使用するアプリケーションの短い説明です。|
|activationUrl | String | 必須。 AppId によって表される最適なネイティブの経験ではアクティビティを起動するために使用する URL です。 ネイティブ アプリケーションが存在しない場合は、web ベースのアプリケーションを起動する場合があります。|
|fallbackUrl | String | 省略可能。 URL が利用可能な場合は、web ベースのアプリケーションでは、アクティビティの起動に使用します。|
|contentUrl | String | 省略可能。 ネイティブまたは web ベースのアプリケーションの操作 (たとえば、RSS フィード内のアイテムへのポインター) の外部コンテンツを表示できる場合に使用されます。|
|visualElements| [visualInfo](../resources/projectrome-visualinfo.md) | 必須。 エクスペリエンスの利用状況を表示する情報を格納しているオブジェクト|
|contentInfo | JSON オブジェクトの型指定されていません。 | 省略可能。 [Schema.org](https://schema.org)の構文に従ってコンテンツの拡張の説明を %ld 個の JSON データのカスタムの一部。|
|expirationDateTime | DateTimeOffset | サーバーで設定します。 オブジェクトは、サーバー上で有効期限が切れたときの utc 日時。|
|status | EnumType | サーバーで設定します。 有効なオブジェクトを識別するために使用する状態コードです。 値: アクティブな場合、更新、削除、無視されます。|

## <a name="relationships"></a>リレーションシップ

|リレーションシップ | 型 | 説明|
|:------------|:-----|:-----------|
|historyItems| [historyItem](../resources/projectrome-historyitem.md)コレクション | 省略可能。 受け取りますおよび抑制ソリューションです。アクティビティの historyItems にナビゲーション プロパティです。|

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
    "status": "EnumType",
    "contentInfo": { "@data.type": "microsoft.graph.Json" },
    "visualElements": { "@data.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.historyItem" }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

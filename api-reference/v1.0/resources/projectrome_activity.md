# <a name="activity-resource-type"></a>アクティビティのリソースの種類

テレビ番組、文書、ビデオ ゲームの現在のキャンペーンなど、アプリケーション内で 1 つのアクティビティを表します。 ユーザーは、そのアクティビティを行っている場合に、そのアクティビティの開始と終了時刻を示す [履歴項目](projectrome_historyitem.md) としてユーザーの行動がキャプチャされます。 ユーザーが時間が経ってから再度、そのアクティビティを行なうにしたがって、1 人のユーザーのアクティビティに対して複数の履歴項目が記録されます。

 Microsoft Graph でのアクティビティを使用して、ユーザーは複数のデバイスにまたがり、アプリでの実行内容を再び取得し直すことができます。 アプリが作成するアクティビティは、すべてのユーザーのデバイスに表示され、アプリ内で特定のコンテンツへのディープ リンクとしてユーザーに公開されます。 Windows で表示され、Cortana の通知を通じて iOS デバイスと Android デバイスにアクセスできる宛先として、アプリ内で特定のコンテンツを表示できます。

すべてのアプリケーションが異なっているため、Cortana および Timeline に表示されるユーザー ・ アクティビティにアプリケーション内の操作をマップする最善の方法を理解できるのはユーザー次第です。 たとえば、ゲームでは、キャンペーンごとのアクティビティ、ドキュメント作成アプリではドキュメント固有のアクティビティ、基幹業務アプリケーションではワークフローごとのアクティビティがそれぞれ作成される可能性があります。

ユーザー アクティビティは Cortana および Windows Timeline に表示されます。これは、過去に従事していたコンテンツに戻れるようにすることで、ユーザーの生産性と効率性の向上に重点を置いています。

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[アクティビティを作成または置換する](../api/projectrome_put_activity.md) | [アクティビティ](projectrome_activity.md) |作成または既存の活動を置換します  (アップサート) 。 AppActivityId は URL セーフである必要があります (RFC 2396 非予約文字以外のすべての文字は 16 進表現に変換する必要があります) 。ただし、元の appActivityId は URL セーフである必要はありません。 |
|[アクティビティを削除する](../api/projectrome_delete_activity.md) | コンテンツなし | アプリから、そのユーザーに対して指定したアクティビティを削除します。|
|[アクティビティを取得する](../api/projectrome_get_activities.md) |  [アクティビティ](projectrome_activity.md)のコレクション | 特定のユーザーに対するアプリのアクティビティを取得します。|
|[最近のアクティビティを取得する](../api/projectrome_get_recent_activities.md) |  [アクティビティ](projectrome_activity.md)のコレクション | 特定のユーザーがアプリで行った最新のアクティビティを、並べ替え後、直近に作成または更新された [historyItems](projectrome_historyitem.md)に基づいて取得します。|

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|userTimezone | 文字列 | 省略可能。 アクティビティの作成時に使用されたユーザーのデバイスがアクティビティ生成時に存在していたタイム ゾーン。クロスプラット フォームの表示に対応するために、Olson Id として指定された値。|
|createdDateTime | DateTimeOffset | サーバーで設定します。 サーバー上でオブジェクトが作成されたときの UTC 日時。 |
|lastModifiedDateTime | DateTimeOffset | サーバーで設定します。 サーバー上でオブジェクトが変更されたときの UTC 日時。 |
|id | 文字列 | サーバーによって生成される ID が URL のアドレスを指定するために使用します。|
|appActivityId | 文字列 | 必須。 アプリのコンテキストにおける一意のアクティビティ ID です。呼び出し元によって提供され、その後不変です。|
|activitySourceHost | 文字列 | 必須。 アプリに対するクロスプラット フォームの id のマッピングを表すドメインの URL です。 マッピングは、ドメインでホストされている JSON ファイルとして保存されるか、Windows デベロッパー センターを使用して構成するかできます。 JSON ファイルは、クロス プラットフォーム アプリケーション識別子として名前がつけられ、HTTPS ドメインのルートでトップ レベルのドメイン レベル、またはサブ ドメインを含むかしてホストされています。 例: https://contoso.com または https://myapp.contoso.com。ただし、https://myapp.contoso.com/somepath は無効です。 クロスプラットフォームのアプリ ID ごとに、一意のファイルおよびドメイン (またはサブ ドメイン) がなくてはなりません。 たとえば、PowerPoint と Word には、別のファイルとドメインが必要です。|
|AppDisplayName | 文字列 | 省略可能。 アプリがユーザーのローカル デバイスにインストールされていない場合に使用するアクティビティを生成するためのアプリの短い文章による説明です。|
|activationUrl | 文字列 | 必須。 appId によって表される最適なネイティブ エクスペリエンスでアクティビティを起動するために使用する URL です。 ネイティブ アプリが存在しない場合、Web ベースのアプリを起動することがあります。|
|fallbackUrl | 文字列 | 省略可能。  使用可能な場合、Web ベースのアプリでのアクティビティの起動に使用する URL です。|
|contentUrl | 文字列 | 省略可能。 ネイティブまたは Web ベースのアプリケーションのエクスペリエンス (たとえば、RSS フィード内のアイテムへのポインター) の外部でコンテンツを表示できる場合に使用されます。|
|visualElements| [visualInfo](../resources/projectrome_visualinfo.md) | 必須。 UX のアクティビティを表示する情報を格納しているオブジェクトです。|
|contentInfo | 型指定されていない JSON オブジェクト | 省略可能。 データのカスタム部分。[schema.org](http://schema.org) 構文に従った、コンテンツの  JSON-LD 拡張記述。|
|expirationDateTime | DateTimeOffset | サーバーで設定します。 サーバー上でオブジェクトの有効期限が切れたときの UTC 日時。|
|status | status | サーバーで設定します。 有効なオブジェクトを識別するために使用する状態コードです。 値: アクティブ、更新、削除、無視。|

## <a name="relationships"></a>リレーションシップ

|リレーションシップ | 型 | 説明|
|:------------|:-----|:-----------|
|historyItems| [activityHistoryItem](../resources/projectrome_historyitem.md) コレクション | 省略可能。 NavigationProperty/Containment。アクティビティの historyItems に対するナビゲーション プロパティです。|

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
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userActivity",
  "@odata.annotations": [
    {
      "capabilities": {
        "countable": false,
        "selectable": false,
        "skippable": false
      }
    }
  ]
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
    "status": "active | updated | deleted | ignored",
    "contentInfo": { "@odata.type": "microsoft.graph.Json" },
    "visualElements": { "@odata.type": "microsoft.graph.visualInfo" },
    "historyItems": [{ "@odata.type": "microsoft.graph.activityHistoryItem" }]
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

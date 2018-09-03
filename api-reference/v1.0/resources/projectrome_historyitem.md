# <a name="historyitem-resource-type"></a>historyItem リソースの種類

アプリ内の [アクティビティ](projectrome_activity.md) の履歴項目を表します。 ユーザーのアクティビティは、アプリ内の単一の宛先 (たとえば、テレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーンなど) を表します。 ユーザーがそのアクティビティを行っている場合、そのアクティビティの開始時刻と終了時刻を示す履歴項目としてユーザーの動作がキャプチャされます。 時間が経過してユーザーがそのアクティビティを再度行うと、複数の履歴項目が 1 人のユーザーのアクティビティに対して記録されます。

アプリがセッションを作成する場合は、**historyItem** オブジェクトを **activity** オブジェクトに追加して、ユーザーの動作期間を反映する必要があります。 ユーザーがアクティビティを再度行うごとに、新しい **historyItem** が追加され、ユーザーの動作が蓄積されます。

## <a name="methods"></a>メソッド

|メソッド | 戻り値の型 | 説明|
|:------|:------------|:-----------|
|[Create or replace historyItem](../api/projectrome_put_historyitem.md) | [historyItem](projectrome_historyitem.md) | その動作の既存の **historyItem** を作成または置換します (UPSERT)。 ID は GUID である必要があります。|
|[Delete a historyItem](../api/projectrome_delete_historyitem.md) | コンテンツなし | そのアクティビティに指定された **historyItem** を削除します。|

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|status | status | サーバーで設定します。 有効なオブジェクトを識別するために使用するステータス コードです。 値は、 active、updated、deleted、ignored です。|
|userTimezone | String | 省略可能。 アクティビティを生成するために使用されたユーザーのデバイスが、アクティビティ作成時に存在していた場所のタイム ゾーンです。 クロス プラットフォームの表示をサポートするために、Olson の ID として指定された値です。|
|createdDateTime | DateTimeOffset | サーバーで設定します。 サーバー上でオブジェクトが作成されたときの UTC の DateTime です。|
|lastModifiedDateTime | DateTimeOffset | サーバーで設定します。 サーバー上でオブジェクトが変更されたときの UTC の DateTime です。|
|id | 文字列 | 必須。  **HistoryItem** オブジェクトのクライアント設定の GUID です。|
|startedDateTime | DateTimeOffset | 必須。  **historyItem** (アクティビティ セッション) が開始されたときの UTC DateTime です。 タイムラインの履歴に必要です。|
|lastActiveDateTime | DateTimeOffset | 省略可能。 **historyItem** (アクティビティ セッション) が最後にアクティブ状態または終了状態と理解されたときの UTC DateTime です。null の場合は、**historyItem** は Ongoing の状態である必要があります。|
|expirationDateTime | DateTimeOffset | 省略可能。  **HistoryItem** が物理削除されるときの UTC DateTime です。 クライアントによって設定できます。|
|activeDurationSeconds | int | 省略可能。 アクティブ ユーザーの動作期間です。 指定されなかった場合、**startedDateTime** と **lastActiveDateTime** から計算されます。|

## <a name="relationships"></a>リレーションシップ

|リレーションシップ | 型 | 説明|
|:------------|:-----|:-----------|
|activity| [userActivity](../resources/projectrome_activity.md) | 省略可能。 NavigationProperty/Containment; 関連するアクティビティのナビゲーション プロパティです。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

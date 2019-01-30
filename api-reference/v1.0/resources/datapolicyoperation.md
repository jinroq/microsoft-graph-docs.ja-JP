# <a name="datapolicyoperation-resource-type"></a>dataPolicyOperation リソースの種類

送信されたデータ ポリシー操作を表します。 操作のステータスを追跡するために必要な情報が含まれています。 など、企業の管理者は、従業員の会社のデータをエクスポートするのにはデータのポリシーの操作要求を送信し、その要求を後で追跡できます。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[DataPolicyOperation を取得します。](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |**DataPolicyOperation**オブジェクトのプロパティを取得します。|
|[個人データをエクスポートします。](../api/user-exportpersonaldata.md) | なし |[DataPolicyOperation の取得](../api/datapolicyoperation-get.md)を使用して後で読み取ることができますが、組織のユーザーのデータをエクスポートするのには、データ ポリシーの操作要求を送信します。|

## <a name="properties"></a>プロパティ

> **注:** このリソースのすべてのプロパティは、読み取り専用です。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|CompletedDateTime|DateTimeOffset|このデータ ポリシーの操作の要求が完了すると、UTC 時刻での ISO 8601 形式を使用して表します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。 操作が完了するまで null になります。|
|id|String| この操作に固有のキーです。 |
|status|string| 可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。|
|storageLocation|String|URL の場所のデータをエクスポートするのには、要求をエクスポートします。|
|userId|String|操作を実行するユーザーのユーザーの id。|
|submittedDateTime|DateTimeOffset|このデータの操作の要求が送信された UTC 時刻での ISO 8601 形式を使用する場合を表します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|進行状況|String|操作の進行状況を指定します。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

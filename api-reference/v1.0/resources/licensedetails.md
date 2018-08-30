# <a name="licensedetails-resource-type"></a>licenseDetails リソースの種類

ユーザーに割り当てられているライセンスに関する情報が含まれています。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[licenseDetails を一覧表示する](../api/user_list_licensedetails.md) | licenseDetails コレクション |ユーザーの licenseDetails オブジェクトの一覧を取得します。|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|ID|文字列| ライセンス詳細オブジェクトの一意識別子。読み取り専用。キー。null 許容ではありません。 |
|servicePlans|[servicePlanInfo](serviceplaninfo.md) コレクション| ライセンスが割り当てられたサービス プランに関する情報。読み取り専用。null 許容ではありません。 |
|skuId|Guid| サービス SKU の一意識別子 (GUID)。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuId プロパティと同じです。読み取り専用 |
|skuPartNumber|文字列| 一意の SKU 表示名です。関連する [SubscribedSku](subscribedsku.md) オブジェクトの skuPartNumber と同じです。例: "AAD_Premium"。読み取り専用 |

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
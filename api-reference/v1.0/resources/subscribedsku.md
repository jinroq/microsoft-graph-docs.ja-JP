# <a name="subscribedsku-resource-type"></a>subscribedSku リソースの種類

会社が購読しているサービス SKU に関する情報が含まれています。

購読している SKU では読み取り操作のみがサポートされ、作成、更新、削除はサポートされません。クエリのフィルター式はサポートされていません。

[directoryObject](directoryobject.md) から継承します。


## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[subscribedSku を取得する](../api/subscribedsku_get.md) | [subscribedSku](subscribedsku.md) |subscribedsku オブジェクトのプロパティを読み取ります。|

## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|capabilityStatus|String|"Enabled"、"LockedOut"、"Suspended" など。|
|consumedUnits|Int32|割り当てられたライセンスの数。|
|id|String|購読している SKU オブジェクトの一意識別子。キー。読み取り専用です。|
|prepaidUnits|[licenseUnitsDetail](licenseunitsdetail.md)|プリペイド ライセンスの数と状態に関する情報。|
|servicePlans|[servicePlanInfo](serviceplaninfo.md) コレクション|SKU と併用できるサービス プランに関する情報。|
|skuId|Guid|サービス SKU の一意識別子 (GUID)。|
|skuPartNumber|String|SKU 部品番号。"AAD_PREMIUM" や "RMSBASIC" など。|
|appliesTo|String|"User" や "Company" など。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

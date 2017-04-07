# <a name="serviceplaninfo-resource-type"></a>servicePlanInfo リソースの種類

購読している SKU に関連付けられているサービス プランに関する情報が含まれています。[subscribedSku](subscribedsku.md) エンティティの **servicePlans** プロパティは、**servicePlanInfo** のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|servicePlanId|Guid|サービス プランの一意識別子。|
|servicePlanName|String|サービス プランの名前。|
|provisioningStatus|String|サービス プランのプロビジョニング状況。|
|appliesTo|String||


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

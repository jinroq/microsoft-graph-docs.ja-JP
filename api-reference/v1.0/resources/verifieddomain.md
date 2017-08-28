# <a name="verifieddomain-resource-type"></a>verifiedDomain リソースの種類

テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|capabilities|String|「電子メール」、「OfficeCommunicationsOnline」など。|
|isDefault|Boolean|                これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。            |
|isInitial|Boolean|これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。|
|name|String|ドメイン名。「contoso.onmicrosoft.com」など。|
|type|String|「管理対象」など。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="persontype-resource-type"></a>personType リソースの種類

個人の種類を表します。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|クラス|String|データ ソースの種類 (Person など)。|
|サブクラス|String|データ ソースの 2 番目の種類 (OrganizationUser など)。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persontype resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

# <a name="timezoneinformation-resource-type"></a>timeZoneInformation リソースの種類


タイム ゾーンを表します。 サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](http://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|alias|string|タイム ゾーンの識別子。|
|displayName|string|タイム ゾーンを表す表示文字列。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
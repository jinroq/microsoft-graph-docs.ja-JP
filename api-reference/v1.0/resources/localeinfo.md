# <a name="localeinfo-resource-type"></a>localeInfo リソースの種類

サインインしているユーザーの優先言語および国/地域を含むロケールに関する情報。


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|locale|string|ユーザーのロケールを表します。ユーザーの優先言語および国/地域が含まれます。たとえば、"en-us"。言語のコンポーネントは [ISO 639-1](http://www.iso.org/iso/home/standards/language_codes.htm) で定義されている 2 文字のコードに従い、国のコンポーネントは [ISO 3166-1 alpha-2](http://www.iso.org/iso/country_codes.htm) で定義されている 2 文字のコードに従います。|
|displayName|string|たとえば "English (United States)" のように、ユーザーのロケールを自然言語で表す名前。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.localeInfo"
}-->

```json
{
  "locale": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "localeInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
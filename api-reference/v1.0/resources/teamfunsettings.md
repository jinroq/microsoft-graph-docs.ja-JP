# <a name="teamfunsettings-resource-type"></a>teamFunSettings リソースの種類



Giphy、memes、および[チーム](team.md)のステッカーを構成する設定を使用します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowGiphy|Boolean|場合 true の場合、有効にする Giphy の使用を設定します。|
|giphyContentRating|文字列 (列挙型)|コンテンツの規制を Giphy。 使用可能な値は、`moderate`、`strict` です。|
|allowStickersAndMemes|Boolean|場合は true、ステッカー、memes など、ユーザーに設定します。|
|allowCustomMemes|Boolean|場合に true を設定する、カスタムの memes を含むようにユーザーをできるようにする設定です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

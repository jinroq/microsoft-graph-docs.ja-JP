# <a name="visualinfo-resource-type"></a>visualInfo リソースの種類

 [activity](../resources/projectrome_activity.md) オブジェクトの **visualElements** プロパティを表すための複合型です。

各ユーザーのアクティビティは、アダプティブ カードとしてタイムラインに表示されます。 アプリ開発者は、アプリ内で行われたアクティビティの概要をキャプチャするカスタム カードを提供するよう奨励されています。 これは、コンテンツ プロパティでカスタム JSON カードを提供することにより可能です。

アダプティブ カードを含むビジュアル メタデータに加えて、アプリは、将来的な再エンゲージメントにつながる新たなアクティビティを提供する目的でユーザーのアクティビティに関する推論を構築するのに使用できるコンテンツ メタデータを指定することができます。 これは、コンテンツを記述するのに schema.org プロパティを利用する JSON オブジェクトを提供する目的で、アクティビティの contentInfo プロパティを使用することにより可能です。

カスタム カードが提供されていない場合は、displayText および description プロパティを使って単純なカードが生成されます。 アプリ内で最高のコンテンツをショーケースするためにカスタム カードが推奨されています。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:------|:-----------|
|displayText | 文字列 | 必須。 ユーザーの一意のアクティビティの簡潔な説明文 (アクティビティがドキュメントの作成を参照する場合は、文書名など)|
|description | 文字列 | 省略可能。 ユーザーのユニーク アクティビティのより長い説明文 (ドキュメント名、最初の文、および / またはメタデータなど)|
|backgroundColor | 文字列 | 省略可能。 UI でアクティビティを示すために使用される背景色で、アクティビティのアプリケーション ソースのブランド色です。 有効な 16 進数の色でなければなりません|
|content | 型指定されていない JSON オブジェクト | 省略可能。 カスタム データ - Windows シェル UI のアクティビティを表示するためのカスタム コンテンツを提供するのに使用される JSON オブジェクト|
|attribution | [imageInfo](../resources/projectrome_imageinfo.md) | 省略可能。 アクティビティを生成するのに使用されるアプリケーションを表すアイコンを示すのに使用される JSON オブジェクト|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attribution",
    "description",
    "backgroundColor",
    "content"
  ],
  "@odata.type": "microsoft.graph.visualInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "String (URL)",
        "alternateText": "String",
        "addImageQuery": "boolean"
    },
    "description": "String",
    "backgroundColor": "String",
    "displayText": "String",
    "content": {
        "@odata.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

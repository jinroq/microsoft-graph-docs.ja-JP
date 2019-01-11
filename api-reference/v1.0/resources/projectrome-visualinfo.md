---
title: visualInfo リソースの種類
description: アクティビティ オブジェクトの**visualElements**プロパティを表すための複合型です。
localization_priority: Normal
ms.openlocfilehash: be40c4718944f1a739a9532a02c3d249514a2a13
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816479"
---
# <a name="visualinfo-resource-type"></a>visualInfo リソースの種類

[アクティビティ](../resources/projectrome-activity.md)オブジェクトの**visualElements**プロパティを表すための複合型です。

各ユーザーの利用状況は、アダプティブ ・ カードとしてタイムラインに表示されます。 アプリの開発者は、アプリケーションで行われた活動の本質をキャプチャするカスタム カードを提供することをお勧めします。 コンテンツのプロパティで、カスタム JSON カードを提供することで可能です。

アプリケーションだけでなく、適応型のカードを使用して visual メタデータは、コンテンツ メタデータ: データを含むを指定できます将来の再契約に新しい活動を提供するためにユーザーのアクティビティの推論を構築するために使用します。 Schema.org のコンテンツを記述するプロパティを利用している JSON オブジェクトを提供するアクティビティの contentInfo プロパティを使用して可能です。

カスタム カードが指定されていない場合、表示テキストと説明のプロパティを使用して単純なカードが生成されます。 カスタム カードはアプリ内での最適なコンテンツの紹介をお勧めします。

## <a name="properties"></a>プロパティ

|名前 | 種類 | 説明|
|:----|:------|:-----------|
|表示テキスト | String | 必須。 ユーザーの一意のアクティビティ (たとえば、アクティビティがドキュメントの作成を参照する場所の場合の文書名) の説明文を短く|
|説明 | String | 省略可能。 ユーザーの固有の活動の長いテキストの説明 (例: ドキュメントの名前、最初の文、またはメタデータ)|
|背景色 | String | 省略可能。 UI のアクティビティのアプリケーションのソースのブランド カラーでアクティビティを表示するために使用する背景色です。 有効な 16 進数の色をする必要があります。|
|content | JSON オブジェクトの型指定されていません。 | 省略可能。 Windows シェル UI のアクティビティを表示するカスタムのコンテンツを提供するカスタムのデータを JSON オブジェクトの使用|
|属性 | [imageInfo](../resources/projectrome-imageinfo.md) | 省略可能。 JSON オブジェクトを使用してアクティビティを生成するアプリケーションを表すアイコンを表すために使用|

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

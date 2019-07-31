---
title: visualInfo リソースの種類
description: Activity オブジェクトの**Visualelements**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 9656252250cf795bcf7c9a1c7682111d7cc37ab1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008874"
---
# <a name="visualinfo-resource-type"></a>visualInfo リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Activity](../resources/projectrome-activity.md)オブジェクトの**visualelements**プロパティを表すための複合型。

各ユーザーアクティビティは、アダプティブカードとしてタイムラインに表示されます。 アプリ開発者は、アプリで行われたアクティビティの本質をキャプチャするカスタムカードを提供することをお勧めします。 これは、コンテンツプロパティにカスタム JSON カードを提供することによって可能になります。

アプリでは、アダプティブカードを使用したビジュアルメタデータに加えて、コンテンツメタデータを指定できます。これにより、ユーザーのアクティビティに対する推論を構築する際に使用されるデータが提供されます。 これは、アクティビティの contentInfo プロパティを使用して、コンテンツを説明するために schema.org プロパティを活用する JSON オブジェクトを提供することによって可能になります。

カスタムカードが提供されていない場合は、表示テキストと説明のプロパティを使用して、簡単なカードが生成されます。 カスタムカードは、アプリ内から最適なコンテンツを示すために推奨されています。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:------|:-----------|
|テキスト | String | 必須。 ユーザーの一意のアクティビティの短いテキスト説明 (たとえば、アクティビティがドキュメントの作成を参照する場合のドキュメント名)。|
|description | String | 省略可能。 ユーザー固有のアクティビティに関する長いテキストの説明 (例: ドキュメント名、最初の文、またはメタデータ)|
|背景 | String | 省略可能。 アクティビティのアプリケーションソースの UI ブランドカラーでアクティビティをレンダリングするために使用される背景色。 有効な16進カラーである必要があります。|
|content | 型指定のない JSON オブジェクト | 省略可能。 Windows シェル UI でアクティビティをレンダリングするためにカスタムコンテンツを提供するために使用されるデータ JSON オブジェクトのカスタム部分|
|帰属 | [imageInfo](../resources/projectrome-imageinfo.md) | 省略可能。 アクティビティの生成に使用されたアプリケーションを表すアイコンを表すために使用される JSON オブジェクト|

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
    "@data.type": "microsoft.graph.visualInfo",
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
        "@data.type": "microsoft.graph.Json"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "visualinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

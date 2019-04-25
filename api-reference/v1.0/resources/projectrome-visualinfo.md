---
title: visualinfo リソースの種類
description: activity オブジェクトの**visualelements**プロパティを表すための複合型。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 416109bb1bb6625330ddfbbb32b8fb688b223134
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579686"
---
# <a name="visualinfo-resource-type"></a>visualinfo リソースの種類

[activity](../resources/projectrome-activity.md)オブジェクトの**visualelements**プロパティを表すための複合型。

各ユーザーアクティビティは、アダプティブカードとしてタイムラインに表示されます。 アプリ開発者は、アプリで行われたアクティビティの本質をキャプチャするカスタムカードを提供することをお勧めします。 これは、コンテンツプロパティにカスタム JSON カードを提供することによって可能になります。

アプリでは、アダプティブカードを使用したビジュアルメタデータに加えて、コンテンツメタデータを指定できます。これにより、ユーザーのアクティビティに対する推論を構築する際に使用されるデータが提供されます。 これは、アクティビティの contentinfo プロパティを使用して、コンテンツを説明するために schema.org プロパティを活用する JSON オブジェクトを提供することによって可能になります。

カスタムカードが提供されていない場合は、表示テキストと説明のプロパティを使用して、簡単なカードが生成されます。 カスタムカードは、アプリ内から最適なコンテンツを示すために推奨されています。

## <a name="properties"></a>プロパティ

|名前 | 型 | 説明|
|:----|:------|:-----------|
|テキスト | String | 必須。 ユーザーの一意のアクティビティの短いテキスト説明 (たとえば、アクティビティがドキュメントの作成を参照する場合のドキュメント名)。|
|説明 | String | 省略可能。 ユーザー固有のアクティビティに関する長いテキストの説明 (例: ドキュメント名、最初の文、またはメタデータ)|
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

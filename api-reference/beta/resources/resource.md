---
title: resource リソースの種類
description: 'イメージまたは OneNote のページ上の他のファイル リソースです。 '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510282"
---
# <a name="resource-resource-type"></a>resource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

イメージまたは OneNote のページ上の他のファイル リソースです。 

リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。

```
GET ../onenote/resources/{id}/content
```

ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。

```
GET ../onenote/pages/{id}/content
```

ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

`object` タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>プロパティ
なし

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リソース バイナリ データの取得](../api/resource-get.md) | Stream |ファイルまたはイメージ リソースのバイナリ データを取得します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

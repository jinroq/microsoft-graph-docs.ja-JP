---
title: OneNoteResource リソースの種類
description: 'OneNote ページ上の画像またはその他のファイルリソース。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cd8ea18047aa3f24343411f8dafd7a79357da87b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034693"
---
# <a name="onenoteresource-resource-type"></a>OneNoteResource リソースの種類

OneNote ページ上の画像またはその他のファイルリソース。 

リソースのバイナリデータを取得することはできますが、リソースオブジェクトまたはリソースコレクションの JSON 表記を取得することはサポートされていません。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

特定のリソースのバイナリデータを取得するために、GET 要求をリソースの`content`エンドポイントに送信します。

```
GET ../onenote/resources/{id}/content
```

ファイルのリソース URI は、次の要求を使用してページの HTML コンテンツを取得したときに返されます。

```
GET ../onenote/pages/{id}/content
```

ページ HTML の場合、 `img`タグには、 `data-fullres-src`属性内の元のイメージリソースのエンドポイントと、 `src`属性の最適化されたイメージが含まれています。
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

`object`タグ (PDF、.DOCX、PNG などのファイルを表す) には、 `data`属性のファイルリソースのエンドポイントが含まれています。

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a>プロパティ

| プロパティ             | 型            | 説明
|:---------------------|:----------------|:---------------------------------
| content              | Stream          | コンテンツストリーム
| contentUrl           | String (url)    | コンテンツをダウンロードするための URL

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リソースバイナリデータの取得](../api/resource-get.md) | Stream |ファイルまたはイメージリソースのバイナリデータを取得します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

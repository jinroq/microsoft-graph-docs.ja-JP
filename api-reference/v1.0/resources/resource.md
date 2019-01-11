---
title: OneNoteResource リソースの種類
description: 'イメージまたは OneNote のページ上の他のファイル リソースです。 '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855105"
---
# <a name="onenoteresource-resource-type"></a>OneNoteResource リソースの種類

イメージまたは OneNote のページ上の他のファイル リソースです。 

リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。

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

| プロパティ             | 種類            | 説明
|:---------------------|:----------------|:---------------------------------
| content              | Stream          | コンテンツ ストリーム
| contentUrl           | 文字列 (url)    | コンテンツをダウンロードするための URL

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リソース バイナリ データの取得](../api/resource-get.md) | Stream |ファイルまたはイメージ リソースのバイナリ データを取得します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

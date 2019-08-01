---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くためのリンクです。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f112d8ff87329ca23a3a44fb33dafe4582072519
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034833"
---
# <a name="recentnotebooklinks-resource-type"></a>recentNotebookLinks リソース型

OneNote ノートブックを開くためのリンクです。 このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。|
|oneNoteWebUrl|[externalLink](externallink.md)|OneNote で web 上のノートブックを開きます。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

---
author: JeremyKelley
description: listInfo 複合型は、list に関する追加情報を提供します。
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 962fc4928bac69489cf2ae2a4c77f3b72169ce0c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966945"
---
# <a name="listinfo-resource"></a>ListInfo リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**listInfo** 複合型は、[list][] に関する追加情報を提供します。

[list]: list.md

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>プロパティ

| プロパティ名           | 種類    | 説明
|:------------------------|:--------|:------------------------------------------------
| **contentTypesEnabled** | Boolean | `true` である場合、このリストのコンテンツ タイプが有効であることを示します。
| **hidden**              | Boolean | `true` である場合、リストが通常 SharePoint ユーザー エクスペリエンスに表示されないことを示します。
| **template**            | String  | リストの作成に使用される基本リスト テンプレートを表す列挙値。 代入可能な値は `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` などです。

### <a name="remarks"></a>備考

ユーザーによって作成されたほとんどのリストには、上記の値のいずれかが含まれますが、それ以外の値を含めることも可能です。
アプリは、ここに記載されていない任意の値も処理できるようになっている必要があります。
SharePoint の CSOM API に詳しい開発者へ: `template` の値は `SPListTemplateType` 列挙体に相当します。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

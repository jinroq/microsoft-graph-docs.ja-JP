---
title: TableSort リソースの種類
description: Table オブジェクトの並べ替え操作を管理します。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 14dbd96567510a3aefab4fddbc57a196c7734b5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033916"
---
# <a name="tablesort-resource-type"></a>TableSort リソースの種類

Table オブジェクトの並べ替え操作を管理します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableSort を取得する](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |tableSort オブジェクトのプロパティと関係を読み取ります。|
|[Apply](../api/tablesort-apply.md)|None|並べ替え操作を実行します。|
|[Clear](../api/tablesort-clear.md)|なし|テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。|
|[Reapply](../api/tablesort-reapply.md)|なし|テーブルに、現在の並べ替えパラメーターを再適用します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fields|[WorkbookSortField](sortfield.md)コレクション|テーブルの最後の並べ替えに使用する現在の条件を表します。 読み取り専用です。|
|matchCase|ブール値|大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。|
|method|string|テーブルの並べ替えで最後に使用した中国語文字の順序付け方法を表します。 使用可能な値は`PinYin`、 `StrokeCount`、です。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

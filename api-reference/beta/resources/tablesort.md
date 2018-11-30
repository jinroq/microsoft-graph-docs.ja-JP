---
title: TableSort リソースの種類
description: テーブル オブジェクトの並べ替え操作を管理します。
ms.openlocfilehash: 02ee1f72bc53a3097c76cf9bab62a165fe3c56f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074396"
---
# <a name="tablesort-resource-type"></a>TableSort リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

テーブル オブジェクトの並べ替え操作を管理します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[TableSort を取得する](../api/tablesort-get.md) | [TableSort](tablesort.md) |tableSort オブジェクトのプロパティと関係を読み取ります。|
|[適用](../api/tablesort-apply.md)|なし|並べ替え操作を実行します。|
|[クリア](../api/tablesort-clear.md)|なし|テーブルに現在設定されている並べ替えをクリアします。これにより表の順序が変更されることはありませんが、ヘッダーのボタンの状態がクリアされます。|
|[Reapply](../api/tablesort-reapply.md)|なし|テーブルに、現在の並べ替えパラメーターを再適用します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|matchCase|ブール値|大文字小文字の区別が、テーブルの最後の並べ替え操作に影響を与えたかどうかを表します。読み取り専用です。|
|method|文字列|テーブルの並べ替えで最後に使用した中国語文字の順序付け方法を表します。可能な値は、`PinYin`、`StrokeCount` です。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|fields|[SortField](sortfield.md)|テーブルの最後の並べ替えに使用する現在の条件を表します。読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
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
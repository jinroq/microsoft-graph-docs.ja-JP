---
title: outlookCategory リソースの種類
description: ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。 Outlook では、ユーザーがマスターリストでカテゴリを定義し、1つ以上のユーザー定義を適用できます。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0e937e7f41816c0d0e9e511854d10fc70fe8a27b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341792"
---
# <a name="outlookcategory-resource-type"></a>outlookCategory リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーが Outlook アイテム (メッセージやイベントなど) をグループ化するために使用できるカテゴリを表します。 Outlook では、ユーザーがマスターリストでカテゴリを定義し、1つまたは複数のユーザー定義の分類項目をアイテムに適用することができます。 

カテゴリを[作成](../api/outlookuser-post-mastercategories.md)してユーザーのマスター カテゴリ リストに定義するには、REST API を使用することができます。 また、[このマスター カテゴリ リストの取得](../api/outlookuser-list-mastercategories.md)、[特定のカテゴリの取得](../api/outlookcategory-get.md)、カテゴリに関連付けられている色の[更新](../api/outlookcategory-update.md)、カテゴリの[削除](../api/outlookcategory-delete.md)などの操作を行うこともできます。 カテゴリをアイテムに適用するには、適用対象とするアイテムの **categories** コレクションに、カテゴリの **displayName** プロパティを割り当てます。
カテゴリに割り当てることができるリソースには、 [contact](contact.md)、 [event](event.md)、 [message](message.md)、 [outlooktask](outlooktask.md)、 [post](post.md)があります。   

各カテゴリを特徴付けるプロパティには、**displayName** と **color** の 2 つがあります。 **displayName** の値は、ユーザーのマスター リスト内で一意でなければなりません。 一方、**color** には一意の値を設定する必要はありません。マスター リストに含まれる複数のカテゴリに、同じ色をマッピングすることができます。 ユーザーのマスター リスト内のカテゴリには、最大 25 種類の色をマッピングできます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|文字列|ユーザーのメールボックス内でカテゴリを識別する一意の名前。 カテゴリが作成された後に、この名前を変更することはできません。 読み取り専用。|
|color|String|カテゴリを特徴付ける、あらかじめ設定された色の定数。定数は、事前定義された 25 種類の色のいずれか 1 つにマッピングされています。 次の注を参照してください。 |

> **注:** **color** に使用できる値は、あらかじめ設定されている `None`、`preset0`、`preset1` などの定数です。 設定済みの定数は、それぞれ 1 つの色にマッピングされています。ただし、実際の色は、カテゴリを表示する Outloook クライアントに依存します。 次の表に、設定済みの各定数に Outlook (デスクトップ クライアント) でマッピングされている色を記載します。 


| 設定済みの定数  | Outlook でマッピングされている色 |
|:---------------|:--------|
| None | マッピングされている色なし |
| Preset0 | 赤 |
| Preset1 | オレンジ |
| Preset2 | 茶 |
| Preset3 | 黄 |
| Preset4 | 緑 |
| Preset5 | 青緑 |
| Preset6 | オリーブ |
| Preset7 | 青 |
| Preset8 | 紫 |
| Preset9 | 深紅 |
| Preset10 | 鋼色 |
| Preset11 | DarkSteel |
| Preset12 | 灰色 |
| Preset13 | DarkGray |
| Preset14 | 黒 |
| Preset15 | DarkRed |
| Preset16 | DarkOrange |
| Preset17 | DarkBrown |
| Preset18 | DarkYellow |
| Preset19 | DarkGreen |
| Preset20 | DarkTeal |
| Preset21 | DarkOlive |
| Preset22 | DarkBlue |
| Preset23 | DarkPurple |
| Preset24 | DarkCranberry |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookCategory"
}-->

```json
{
  "color": "String",
  "displayName": "String"
}

```

## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[カテゴリの一覧表示](../api/outlookuser-list-mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) コレクション |ユーザーに対して定義されているすべてのカテゴリを取得します。|
|[カテゴリの取得](../api/outlookcategory-get.md) | [outlookCategory](../resources/outlookcategory.md) |指定した **outlookCategory** オブジェクトのプロパティとリレーションシップを取得します。|
|[作成](../api/outlookuser-post-mastercategories.md) | [outlookCategory](../resources/outlookcategory.md) |ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。|
|[更新](../api/outlookcategory-update.md) | [outlookCategory](../resources/outlookcategory.md) |指定した **outlookCategory** オブジェクトの書き込み可能な **color** プロパティを更新します。 |
|[削除](../api/outlookcategory-delete.md) | なし |指定した **outlookCategory** オブジェクトを削除します。 |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/outlookcategory.md:\r\n      Failed to parse any rows out of table with headers: |Pre-set constant|Color mapped to in Outlook|"
  ]
}
-->
 

---
title: businessflowtemplate リソースの種類
description: azure ad access レビュー機能では、は`businesFlowTemplate` azure ad ビジネスフローテンプレートを表します。 グループのゲストメンバーを確認するなどのテンプレートの識別子は、アクセスレビューを作成するときに発信者によって提供されます。
localization_priority: Normal
ms.openlocfilehash: 0cca72bc8ccd372cdaf9952b385bc63f81b0631d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338831"
---
# <a name="businessflowtemplate-resource-type"></a>businessflowtemplate リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

azure ad [access レビュー](accessreviews-root.md)機能では、は`businesFlowTemplate` azure ad ビジネスフローテンプレートを表します。 グループのゲストメンバーを確認するなどのテンプレートの識別子は、アクセスレビューを作成するときに発信者によって提供されます。

ビジネスフローテンプレートオブジェクトは、グローバル管理者がテナントを介してアクセスレビュー機能を使用すると、自動的に生成されます。  追加のビジネスフローテンプレートを作成することはできません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[businessflowtemplates を一覧表示する](../api/businessflowtemplate-list.md) | [businessflowtemplate](businessflowtemplate.md)コレクション| レビューにアクセスするための適切なビジネスフローテンプレートを取得します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | ビジネスフローテンプレートの機能割り当て識別子                                      |
| `displayName`            |`String`                | ビジネスフローテンプレートの名前                                                             |


## <a name="relationships"></a>リレーションシップ

なし。

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[accessreview を作成する](../api/accessreview-create.md) | [accessreview](accessreview.md) |   新しい accessreview を作成します。 |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

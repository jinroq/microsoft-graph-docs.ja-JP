---
title: businessflowtemplate リソースの種類
description: azure ad access レビュー機能では、は`businesFlowTemplate` azure ad ビジネスフローテンプレートを表します。 グループのゲストメンバーを確認するなどのテンプレートの識別子は、アクセスレビューを作成するときに発信者によって提供されます。
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543739"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

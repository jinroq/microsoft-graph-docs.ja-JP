---
title: programcontroltype リソースの種類
description: 'Azure AD access のレビュー機能では、プログラムにコントロールを関連付けるときにコントロールの種類としてコントロールを使用し、コントロールのアクセスレビューの種類を指定します。  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563327"
---
# <a name="programcontroltype-resource-type"></a>programcontroltype リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD access の[レビュー](accessreviews-root.md)機能では、プログラムにコントロールを関連付けるときにコントロールの種類としてコントロールを使用し、コントロールのアクセスレビューの種類を指定します。  

プログラムコントロールの種類のオブジェクトは、グローバル管理者がテナントを介してアクセスレビュー機能を使用するときに自動的に生成されます。  他のプログラムコントロールの種類を作成することはできません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[programcontroltypes のリスト](../api/programcontroltype-list.md) | [programcontroltype](programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | プログラムコントロール型の機能割り当て識別子                                      |
| `displayName`            |`String`                | プログラムコントロールの種類の名前。                                                             |


## <a name="relationships"></a>リレーションシップ

なし。


## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[programcontrol を作成する](../api/programcontrol-create.md) |     [programcontrol](programcontrol.md) |   プログラムに programcontrol を追加します。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
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
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

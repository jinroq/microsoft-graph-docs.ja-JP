---
title: programControlType リソースの種類
description: 'Azure AD access のレビュー機能では、プログラムにコントロールを関連付けるときにコントロールの種類としてコントロールを使用し、コントロールのアクセスレビューの種類を指定します。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c7b4360ffa22711c9af9961fbb9f48cee7d29424
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965629"
---
# <a name="programcontroltype-resource-type"></a>programControlType リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD access の[レビュー](accessreviews-root.md)機能では、プログラムにコントロールを関連付けるときにコントロールの種類としてコントロールを使用し、コントロールのアクセスレビューの種類を指定します。  

プログラムコントロールの種類のオブジェクトは、グローバル管理者がテナントを介してアクセスレビュー機能を使用するときに自動的に生成されます。  他のプログラムコントロールの種類を作成することはできません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ProgramControlTypes のリスト](../api/programcontroltype-list.md) | [Programcontroltype](programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |

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
|[ProgramControl を作成する](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   プログラムに programControl を追加します。|


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

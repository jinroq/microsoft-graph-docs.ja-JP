---
title: programControlType リソースの種類
description: 'Azure AD にアクセスが機能を確認、アクセス確認の種類を示すために、プログラムにコントロールをコントロールに関連付けることが、ときにプログラムのコントロールの種類を使用します。  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070456"
---
# <a name="programcontroltype-resource-type"></a>programControlType リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

機能では、Azure AD[アクセスの確認](accessreviews-root.md)は、プログラムのコントロールの種類はコントロールは、アクセス確認の種類を示すためにも、プログラムにコントロールを関連付ける場合に使用されます。  

プログラムのコントロール型オブジェクトは、グローバル管理者 onboards アクセスを使用するテナント機能を確認するときに自動的に生成されます。  コントロールの種類を追加したプログラムは作成されません。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リスト programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)コレクション| プログラムのコントロールの種類を一覧表示します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | プログラムのコントロールの種類の機能に割り当てられた識別子                                      |
| `displayName`            |`String`                | プログラムのコントロールの種類の名前                                                             |


## <a name="relationships"></a>リレーションシップ

なし。


## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[デバッギングを作成します。](../api/programcontrol-create.md) |     [デバッギング](programcontrol.md) |   デバッギングをプログラムに追加します。|


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

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

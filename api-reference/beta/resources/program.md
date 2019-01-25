---
title: プログラムのリソースの種類
description: 'Azure AD にアクセスが機能を確認、プログラムは、プログラムのコントロールを保持しているコンテナーです。 テナントは、1 つまたは複数のプログラムを持つことができます。  各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515189"
---
# <a name="program-resource-type"></a>プログラムのリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムは、プログラムのコントロールを保持している、コンテナーです。 テナントは、1 つまたは複数のプログラムを持つことができます。  各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。  

各テナントが上に直行し、Azure AD がアクセスのレビューには 1 つのプログラムでは、 `Default program`。  グローバル管理者は、コンプライアンス ・ イニシアティブを表現するなど、その他のプログラムを作成できます。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムを作成します。](../api/program-create.md) |   [プログラム](program.md)   |   新しいプログラムを作成します。|
|[プログラムを削除します。](../api/program-delete.md) |   なし。   |   プログラムを削除します。|
|[プログラムを一覧表示](../api/program-list.md) |  [プログラム](program.md)のコレクション|   すべてのプログラムのコレクションを取得します。|
|[プログラムのリスト programControls](../api/program-listcontrols.md) |      [デバッギング](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[更新プログラム](../api/program-update.md) |   [プログラム](program.md)|  プログラムを更新します。|

## <a name="permissions"></a>アクセス許可

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | ProgramControl.Read.All、ProgramControl.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  プログラムの機能に割り当てられる識別子です。                    |
| `displayName`               |`String`                              |  プログラムの名前です。  必要なを作成します。                  |
| `description`               |`String`                              |  プログラムの説明です。           |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `controls`                  |[デバッギング](programcontrol.md) | プログラムに関連付けられているコントロール。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

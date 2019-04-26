---
title: program リソースの種類
description: 'Azure AD access のレビュー機能であるプログラムは、プログラムコントロールを保持するコンテナーです。 テナントには、1つ以上のプログラムを含めることができます。  各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563411"
---
# <a name="program-resource-type"></a>program リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD access の[レビュー](accessreviews-root.md)機能であるプログラムは、プログラムコントロールを保持するコンテナーです。 テナントには、1つ以上のプログラムを含めることができます。  各コントロールは、アクセスレビューをプログラムにリンクして、関連するアクセスレビューを簡単に見つけられるようにします。  

boarded Azure AD アクセスレビューを持つ各テナントには、 `Default program`1 つのプログラムがあります。  グローバル管理者は、コンプライアンスイニシアチブを表すなど、追加のプログラムを作成できます。 


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムを作成する](../api/program-create.md) |   [アプリケーション](program.md)   |   新しいプログラムを作成します。|
|[プログラムの削除](../api/program-delete.md) |   なし。   |   プログラムを削除します。|
|[プログラムの一覧表示](../api/program-list.md) |  [プログラム](program.md)コレクション|   すべてのプログラムのコレクションを取得します。|
|[プログラムの programcontrols を一覧表示する](../api/program-listcontrols.md) |      [programcontrol](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[プログラムの更新](../api/program-update.md) |   [アプリケーション](program.md)|  プログラムを更新します。|

## <a name="permissions"></a>アクセス許可

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | programcontrol. all、programcontrol. |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  プログラムの機能割り当て識別子。                    |
| `displayName`               |`String`                              |  プログラムの名前を指定します。  作成時に必要です。                  |
| `description`               |`String`                              |  プログラムの説明。           |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `controls`                  |[programcontrol](programcontrol.md) | プログラムに関連付けられているコントロール。 |

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

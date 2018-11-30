---
title: プログラムのリソースの種類
description: 'Azure AD にアクセスが機能を確認、プログラムは、プログラムのコントロールを保持しているコンテナーです。 テナントは、1 つまたは複数のプログラムを持つことができます。  各コントロールは、アクセス確認をプログラムにリンク、関連のアクセスを見つけやすくすることを確認します。  '
ms.openlocfilehash: cb08d0edb7487be95e159ed5e2a2546a92e7bce7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073665"
---
# <a name="program-resource-type"></a>プログラムのリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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

## <a name="permissions"></a>Permissions

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

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
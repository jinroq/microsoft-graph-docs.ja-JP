---
title: デバッギングのリソースの種類
description: Azure AD にアクセスが機能を確認、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンクするコントロールを表します。
localization_priority: Normal
ms.openlocfilehash: 3d9829b8e2585d4deda95551021e2fd9b8d14c7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511416"
---
# <a name="programcontrol-resource-type"></a>デバッギングのリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD[アクセスの確認](accessreviews-root.md)機能では、プログラムのコントロール オブジェクトは、アクセス確認をプログラムにリンク、コントロールを表します。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[デバッギングを作成します。](../api/programcontrol-create.md) |     [デバッギング](programcontrol.md) |   デバッギングをプログラムに追加します。|
|[デバッギングを削除します。](../api/programcontrol-delete.md) |     なし。   |   デバッギングをプログラムから削除します。|
|[リスト programControls](../api/programcontrol-list.md) | [デバッギング](programcontrol.md)コレクション| テナント内のすべてのプログラム間でコントロールを一覧表示します。|

## <a name="permissions"></a>アクセス許可

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | ProgramControl.Read.All、ProgramControl.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                     |`String`                | プログラムとコントロール間のリンクの機能に割り当てられた識別子                                      |
| `programId`              |`String`                | プログラムの programId このコントロールは、一部です。 必要なを作成します。                            |
| `controlId`              |`String`                | コントロールの処理、特にアクセスの id を確認します。 必要なを作成します。                                                |
| `controlTypeId`          |`String`                | ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。 必要なを作成します。 |
| `displayName`            |`String`                | コントロールの名前です。                                                             |
| `status`                 |`String`                | コントロールのライフ サイクルの状態です。                                                 |
| `createdDateTime`        |`DateTimeOffset`        | 作成日付と時刻のコントロールです。                                        |
| `owner`                  |%__UserIdentity__%   | プログラムのコントロールを作成したユーザー。                                               |
| `resource`               |`programResource`       | リソース、グループ、または、アプリケーションは、このプログラムの制御のアクセスの確認の対象となります。                   |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `program`                |[プログラム](program.md)               | このコントロールの一部であるプログラムです。                                                |

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムのリスト programControls](../api/program-listcontrols.md) |      [デバッギング](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[リスト programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)コレクション| プログラムのコントロールの種類を一覧表示します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControl"
}-->

```json
{
 "id": "string (identifier)",
 "programId": "string (identifier)",
 "controlId": "string (identifier)",
 "controlTypeId": "string (identifier)",
 "displayName": "string",
 "status": "string",
 "createdDateTime": "string (timestamp)",
 "owner": "microsoft.graph.userIdentity",
 "resource":"microsoft.graph.programResource"
}

```

## <a name="the-programresource-complex-type"></a>ProgramResource 複合型

プログラム コントロール オブジェクトに含まれている、プログラムのリソースは、アクセス確認の対象であるオブジェクトへの参照の表現です。

このタイプから継承`microsoft.graph.identity`があり、1 つの追加のプロパティ。

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `type`               |`String`  | グループ、またはアプリケーションがあるかどうかを示す、リソースの種類です。 |     


<!--
{
  "type": "#page.annotation",
  "description": "programControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontrol.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
